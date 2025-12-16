<script>
	import logo from '$lib/assets/logo.png';
	import { base } from '$app/paths';

	const fileName = 'MindChips_2025-12-16_08-00-24.zip'
	const downloadUrl = `${base}/MindChips_2025-12-16_08-00-24.zip`

	function handleDownload() {
		const link = document.createElement('a');
		link.href = downloadUrl;
		link.download = fileName;
		document.body.appendChild(link);
		link.click();
		document.body.removeChild(link);
	}
</script>

<svelte:head>
	<title>Download MindChips - AI Desktop Client for macOS</title>
	<meta name="description" content="Download MindChips, the native macOS AI desktop client. Fast, lightweight, and privacy-focused." />
</svelte:head>

<div class="container">
	<!-- Header Section -->
	<section class="header">
		<div class="header-content">
			<img src={logo} alt="MindChips Logo" class="logo" />
			<h1 class="title">Download MindChips</h1>
			<p class="subtitle">Get the latest version of MindChips for macOS</p>
		</div>
	</section>

	<!-- Download Section -->
	<section class="download-section">
		<div class="download-content">
			<div class="download-card">
				<div class="download-icon">📦</div>
				<h2 class="download-title">MindChips for macOS</h2>
				<p class="download-version">Version: 2025-12-14</p>
				<p class="download-description">
					Download the native macOS application and start using AI directly from your desktop.
					The download includes everything you need to get started.
				</p>

				<div class="download-info">
					<div class="info-item">
						<span class="info-label">File Size:</span>
						<span class="info-value">~3.0 MB</span>
					</div>
					<div class="info-item">
						<span class="info-label">Platform:</span>
						<span class="info-value">macOS</span>
					</div>
					<div class="info-item">
						<span class="info-label">Format:</span>
						<span class="info-value">ZIP Archive</span>
					</div>
				</div>

				<button class="download-button" on:click={handleDownload}>
					<span class="button-icon">⬇️</span>
					<span class="button-text">Download Now</span>
				</button>

				<p class="download-note">
					Or <a href={downloadUrl} download={fileName} class="download-link">click here</a> to download directly
				</p>
			</div>

			<div class="instructions">
				<h3 class="instructions-title">Installation Instructions</h3>
				<ol class="instructions-list">
					<li>Download the ZIP file using the button above</li>
					<li>Extract the ZIP file to your desired location</li>
					<li>Open the extracted folder and locate the MindChips application</li>
					<li>Drag the MindChips app to your Applications folder</li>
					<li>Launch MindChips from your Applications folder</li>
				</ol>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="footer">
		<div class="footer-content">
			<p class="footer-text">© 2025 Scrapmind.com All rights reserved.</p>
			<div class="footer-links">
				<a href="{base}/" class="footer-link">Home</a>
				<span class="separator">|</span>
				<a href="{base}/privacy" class="footer-link">Privacy Policy</a>
			</div>
		</div>
	</footer>
</div>

<style>
	:global(body) {
		margin: 0;
		padding: 0;
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
		background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
		min-height: 100vh;
		color: #333;
	}

	.container {
		max-width: 900px;
		margin: 0 auto;
		padding: 0 20px;
	}

	/* Header Section */
	.header {
		padding: 60px 0 80px;
		text-align: center;
		color: white;
	}

	.header-content {
		max-width: 800px;
		margin: 0 auto;
	}

	.logo {
		width: 96px;
		height: 96px;
		margin-bottom: 30px;
		border-radius: 20px;
		box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
		background: white;
		padding: 6px;
	}

	.title {
		font-size: 3rem;
		font-weight: 700;
		margin: 0 0 20px;
		letter-spacing: -0.02em;
		text-shadow: 0 2px 20px rgba(0, 0, 0, 0.2);
	}

	.subtitle {
		font-size: 1.3rem;
		font-weight: 300;
		margin: 0;
		opacity: 0.95;
		line-height: 1.6;
	}

	/* Download Section */
	.download-section {
		background: white;
		border-radius: 30px 30px 0 0;
		margin-top: -40px;
		position: relative;
		z-index: 1;
		padding: 60px 40px;
		min-height: calc(100vh - 300px);
	}

	.download-content {
		max-width: 700px;
		margin: 0 auto;
	}

	.download-card {
		background: #f8f9fa;
		border-radius: 20px;
		padding: 50px 40px;
		text-align: center;
		margin-bottom: 40px;
		border: 1px solid #e9ecef;
		box-shadow: 0 4px 20px rgba(0, 0, 0, 0.05);
	}

	.download-icon {
		font-size: 4rem;
		margin-bottom: 20px;
	}

	.download-title {
		font-size: 2rem;
		font-weight: 700;
		margin: 0 0 10px;
		color: #333;
	}

	.download-version {
		font-size: 1rem;
		color: #667eea;
		font-weight: 600;
		margin: 0 0 20px;
	}

	.download-description {
		font-size: 1rem;
		line-height: 1.7;
		color: #555;
		margin: 0 0 30px;
	}

	.download-info {
		display: flex;
		justify-content: center;
		gap: 40px;
		margin: 30px 0;
		flex-wrap: wrap;
	}

	.info-item {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 5px;
	}

	.info-label {
		font-size: 0.85rem;
		color: #999;
		text-transform: uppercase;
		letter-spacing: 0.5px;
	}

	.info-value {
		font-size: 1.1rem;
		font-weight: 600;
		color: #333;
	}

	.download-button {
		background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
		color: white;
		border: none;
		border-radius: 12px;
		padding: 18px 40px;
		font-size: 1.2rem;
		font-weight: 600;
		cursor: pointer;
		transition: transform 0.2s ease, box-shadow 0.2s ease;
		display: inline-flex;
		align-items: center;
		gap: 10px;
		margin: 20px 0;
		box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4);
	}

	.download-button:hover {
		transform: translateY(-2px);
		box-shadow: 0 6px 20px rgba(102, 126, 234, 0.5);
	}

	.download-button:active {
		transform: translateY(0);
	}

	.button-icon {
		font-size: 1.3rem;
	}

	.button-text {
		letter-spacing: 0.5px;
	}

	.download-note {
		font-size: 0.9rem;
		color: #999;
		margin: 20px 0 0;
	}

	.download-link {
		color: #667eea;
		text-decoration: none;
		font-weight: 500;
		transition: color 0.3s ease;
	}

	.download-link:hover {
		color: #764ba2;
		text-decoration: underline;
	}

	.instructions {
		background: white;
		border-radius: 15px;
		padding: 30px;
		border: 1px solid #e9ecef;
	}

	.instructions-title {
		font-size: 1.5rem;
		font-weight: 700;
		margin: 0 0 20px;
		color: #333;
	}

	.instructions-list {
		margin: 0;
		padding-left: 25px;
		color: #555;
	}

	.instructions-list li {
		font-size: 1rem;
		line-height: 1.8;
		margin-bottom: 12px;
	}

	/* Footer */
	.footer {
		background: #1a1a1a;
		color: white;
		padding: 40px 0 30px;
		margin-top: -40px;
	}

	.footer-content {
		max-width: 800px;
		margin: 0 auto;
		text-align: center;
	}

	.footer-text {
		font-size: 0.9rem;
		color: #999;
		margin: 0 0 20px;
	}

	.footer-links {
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 15px;
	}

	.footer-link {
		color: #667eea;
		text-decoration: none;
		font-size: 0.95rem;
		transition: color 0.3s ease;
	}

	.footer-link:hover {
		color: #764ba2;
		text-decoration: underline;
	}

	.separator {
		color: #666;
	}

	/* Responsive Design */
	@media (max-width: 768px) {
		.title {
			font-size: 2rem;
		}

		.subtitle {
			font-size: 1.1rem;
		}

		.download-section {
			padding: 40px 20px;
		}

		.download-card {
			padding: 40px 25px;
		}

		.download-title {
			font-size: 1.6rem;
		}

		.download-info {
			gap: 30px;
		}

		.download-button {
			padding: 16px 30px;
			font-size: 1.1rem;
			width: 100%;
			justify-content: center;
		}

		.instructions {
			padding: 25px 20px;
		}

		.header {
			padding: 40px 0 60px;
		}

		.logo {
			width: 80px;
			height: 80px;
		}
	}
</style>

