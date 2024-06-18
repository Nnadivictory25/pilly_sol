<script>
	import '../app.css';
	let title = '$PEPILLY | Home';
	let desc = '$PEPE + $BILLY = $PEPILLY';
</script>

<svelte:head>
	<link rel="preload" href="/pepe.png" as="image" />
	<link rel="preload" href="/billy.webp" as="image" />
	<link rel="preload" href="/pilly.jpg" as="image" />

	<title>{title}</title>
	<meta name="description" content={desc} />

	<meta property="og:url" content="https://www.pepilly.xyz" />
	<meta property="og:type" content="website" />
	<meta property="og:title" content={title} />
	<meta property="site_name" content="$PEPILLY" />
	<meta property="og:description" content={desc} />
	<meta property="og:image" content="https://www.pepilly.xyz/og.png" />

	<meta name="twitter:card" content="summary_large_image" />
	<meta property="twitter:domain" content="aistudybud.online" />
	<meta property="twitter:url" content="https://www.pepilly.xyz" />
	<meta name="twitter:title" content={title} />
	<meta name="twitter:description" content={desc} />
	<meta name="twitter:image" content="https://www.pepilly.xyz/og.png" />

	<link rel="canonical" href="https://www.pepilly.xyz" />
	<meta name="robots" content="index, follow" />
	<meta name="googlebot" content="index, follow" />
</svelte:head>
<slot />
