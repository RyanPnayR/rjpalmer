<script lang="ts">
	import '../app.pcss';
	let x = 0;
	let y = 0;
	function mouseHandler(t: { currentTarget: any; clientX: any; clientY: any }) {
		let { currentTarget: e, clientX: i, clientY: n } = t;
		let { left: r, top: o } = e.getBoundingClientRect();
		x = i - r;
		y = n - o;
	}
</script>

<body
	class="bg-slate-900 leading-relaxed text-slate-400 antialiased selection:bg-teal-300 selection:text-teal-900"
>
	<div>
		<div class="group/spotlight relative" role="article" on:mousemove={mouseHandler}>
			<div
				class="pointer-events-none fixed inset-0 z-30 transition duration-300 lg:absolute"
				style="background: radial-gradient(600px at {x}px {y}px, rgba(29, 78, 216, 0.15), transparent 80%);"
			></div>
			<slot />
		</div>
	</div>
</body>
