# auth
 <!doctype html>
    <html lang="en">
      <head>
        <meta charset="UTF-8" />
        <link rel="icon" type="image/svg+xml" href="/vite.svg" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <meta name="description" content="Lydell Tech Solutions - Your premier destination for tech products and professional services. Discover cutting-edge solutions for your business needs." />
        <meta name="keywords" content="tech marketplace, professional services, IT solutions, tech products, business solutions, cloud services, cybersecurity, AI solutions, data analytics" />
        <meta name="author" content="Lydell Tech Solutions" />
        <meta property="og:title" content="Lydell Tech Solutions - Premium Tech Products & Services" />
        <meta property="og:description" content="Your premier destination for tech products and professional services. Transform your business with our cutting-edge solutions." />
        <meta property="og:type" content="website" />
        <meta property="og:image" content="https://storage.googleapis.com/hostinger-horizons-assets-prod/3935a396-ab84-4916-86a0-cc6b6adb5415/20f201c777cacdb774574cb6c6d09210.png" />
        <meta name="twitter:card" content="summary_large_image" />
        <meta name="twitter:title" content="Lydell Tech Solutions" />
        <meta name="twitter:description" content="Premium tech products and professional services for your business success" />
        <meta name="twitter:image" content="https://storage.googleapis.com/hostinger-horizons-assets-prod/3935a396-ab84-4916-86a0-cc6b6adb5415/20f201c777cacdb774574cb6c6d09210.png" />
        <meta name="robots" content="index, follow" />
        <meta name="googlebot" content="index, follow" />
        <link rel="canonical" href="https://lydelltechsolutions.com" />
        <title>Lydell Tech Solutions - Premium Tech Products & Services</title>
        
        <!-- Google tag (gtag.js) -->
        <script async src="https://www.googletagmanager.com/gtag/js?id=G-P5B2DVVQC1"></script>
        <script>
          window.dataLayer = window.dataLayer || [];
          function gtag(){dataLayer.push(arguments);}
          gtag('js', new Date());
        
          gtag('config', 'G-P5B2DVVQC1');
        </script>
        <script type="module" crossorigin src="/assets/index-3cd28c9f.js"></script>
        <link rel="stylesheet" href="/assets/index-2a1fffaa.css">
        <script type="module">
window.onerror = (message, source, lineno, colno, errorObj) => {
	const errorDetails = errorObj ? JSON.stringify({
		name: errorObj.name,
		message: errorObj.message,
		stack: errorObj.stack,
		source,
		lineno,
		colno,
	}) : null;

	window.parent.postMessage({
		type: 'horizons-runtime-error',
		message,
		error: errorDetails
	}, '*');
};
</script>
        <script type="module">
const observer = new MutationObserver((mutations) => {
	for (const mutation of mutations) {
		for (const addedNode of mutation.addedNodes) {
			if (
				addedNode.nodeType === Node.ELEMENT_NODE &&
				(
					addedNode.tagName?.toLowerCase() === 'vite-error-overlay' ||
					addedNode.classList?.contains('backdrop')
				)
			) {
				handleViteOverlay(addedNode);
			}
		}
	}
});

observer.observe(document.documentElement, {
	childList: true,
	subtree: true
});

function handleViteOverlay(node) {
	if (!node.shadowRoot) {
		return;
	}

	const backdrop = node.shadowRoot.querySelector('.backdrop');

	if (backdrop) {
		const overlayHtml = backdrop.outerHTML;
		const parser = new DOMParser();
		const doc = parser.parseFromString(overlayHtml, 'text/html');
		const messageBodyElement = doc.querySelector('.message-body');
		const fileElement = doc.querySelector('.file');
		const messageText = messageBodyElement ? messageBodyElement.textContent.trim() : '';
		const fileText = fileElement ? fileElement.textContent.trim() : '';
		const error = messageText + (fileText ? ' File:' + fileText : '');

		window.parent.postMessage({
			type: 'horizons-vite-error',
			error,
		}, '*');
	}
}
</script>
        <script type="module">
const originalConsoleError = console.error;
console.error = function(...args) {
	originalConsoleError.apply(console, args);

	let errorString = '';

	for (let i = 0; i < args.length; i++) {
		const arg = args[i];
		if (arg instanceof Error) {
			errorString = arg.stack || `${arg.name}: ${arg.message}`;
			break;
		}
	}

	if (!errorString) {
		errorString = args.map(arg => typeof arg === 'object' ? JSON.stringify(arg) : String(arg)).join(' ');
	}

	window.parent.postMessage({
		type: 'horizons-console-error',
		error: errorString
	}, '*');
};
</script>
        <script type="module">
const originalFetch = window.fetch;

window.fetch = function(...args) {
	const url = args[0] instanceof Request ? args[0].url : args[0];

	// Skip WebSocket URLs
	if (url.startsWith('ws:') || url.startsWith('wss:')) {
		return originalFetch.apply(this, args);
	}

	return originalFetch.apply(this, args)
		.then(async response => {
			const contentType = response.headers.get('Content-Type') || '';

			// Exclude HTML document responses
			const isDocumentResponse =
				contentType.includes('text/html') ||
				contentType.includes('application/xhtml+xml');

			if (!response.ok && !isDocumentResponse) {
					const responseClone = response.clone();
					const errorFromRes = await responseClone.text();
					const requestUrl = response.url;
					console.error(`Fetch error from ${requestUrl}: ${errorFromRes}`);
			}

			return response;
		})
		.catch(error => {
			if (!url.match(/.html?$/i)) {
				console.error(error);
			}

			throw error;
		});
};
</script>
      </head>
      <body>
        <div id="root"></div>
        
      </body>
    </html>
  
