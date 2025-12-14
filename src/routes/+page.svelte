<script>
	import logo from '$lib/assets/logo.png';
	import screenshot from '$lib/assets/1280.png';
</script>

<svelte:head>
	<title>MindChips - AI Desktop Client for macOS</title>
	<meta name="description" content="Unlock the power of AI directly from your desktop. MindChips is a native macOS client designed for speed and efficiency." />
</svelte:head>

<div class="container">
	<!-- Hero Section -->
	<section class="hero">
		<div class="hero-content">
			<img src={logo} alt="MindChips Logo" class="logo" />
			<h1 class="title">MindChips</h1>
			<p class="subtitle">Unlock the power of AI directly from your desktop</p>
			<p class="description">
				MindChips is a native macOS client designed for speed and efficiency. Enjoy a lightweight experience with seamless multi-device sync, all while keeping your data private and secure.
			</p>
			<div class="hero-actions">
				<a href="/download" class="download-button">Download Now</a>
			</div>
		</div>
	</section>

	<!-- Screenshot Section -->
	<section class="screenshot-section">
		<div class="screenshot-container">
			<h2 class="screenshot-title">See MindChips in Action</h2>
			<p class="screenshot-subtitle">Experience the intuitive interface designed for seamless AI interactions</p>
			<div class="screenshot-wrapper">
				<img src={screenshot} alt="MindChips Application Screenshot" class="screenshot" />
			</div>
		</div>
	</section>

	<!-- Features Section -->
	<section class="features">
		<h2 class="section-title">Why Choose MindChips?</h2>
		<div class="features-grid">
			<div class="feature-card">
				<div class="feature-icon">🍎</div>
				<div class="feature-card-content">
					<h3 class="feature-title">Native Experience</h3>
					<p class="feature-description">Built specifically for macOS</p>
				</div>
			</div>
			<div class="feature-card">
				<div class="feature-icon">⚡</div>
				<div class="feature-card-content">
					<h3 class="feature-title">Lightweight</h3>
					<p class="feature-description">Minimal disk usage</p>
				</div>
			</div>
			<div class="feature-card">
				<div class="feature-icon">🚀</div>
				<div class="feature-card-content">
					<h3 class="feature-title">Blazing Fast</h3>
					<p class="feature-description">Optimized for best performance</p>
				</div>
			</div>
			<div class="feature-card">
				<div class="feature-icon">🔄</div>
				<div class="feature-card-content">
					<h3 class="feature-title">Seamless Sync</h3>
					<p class="feature-description">Keep your data across all devices</p>
				</div>
			</div>
			<div class="feature-card">
				<div class="feature-icon">🔒</div>
				<div class="feature-card-content">
					<h3 class="feature-title">Privacy First</h3>
					<p class="feature-description">Your data stays yours</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="footer">
		<div class="footer-content">
			<p class="footer-text">© 2025 Scrapmind.com  All rights reserved.</p>
			<div class="footer-links">
				<a href="/privacy" class="footer-link">Privacy Policy</a>
			</div>
			<div class="contact">
				<h3 class="contact-title">Contact Us</h3>
				<p class="contact-info">
					Email: <a href="mailto:pochonlee@gmail.com">pochonlee#gmail.com</a>
				</p>
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
		max-width: 1200px;
		margin: 0 auto;
		padding: 0 20px;
	}

	/* Hero Section */
	.hero {
		padding: 80px 0 100px;
		text-align: center;
		color: white;
	}

	.hero-content {
		max-width: 800px;
		margin: 0 auto;
	}

	.logo {
		width: 128px;
		height: 128px;
		margin-bottom: 30px;
		border-radius: 24px;
		box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
		background: white;
		padding: 8px;
	}

	.title {
		font-size: 4rem;
		font-weight: 700;
		margin: 0 0 20px;
		letter-spacing: -0.02em;
		text-shadow: 0 2px 20px rgba(0, 0, 0, 0.2);
	}

	.subtitle {
		font-size: 1.5rem;
		font-weight: 300;
		margin: 0 0 30px;
		opacity: 0.95;
	}

	.description {
		font-size: 1.1rem;
		line-height: 1.8;
		margin: 0 0 40px;
		opacity: 0.9;
		max-width: 700px;
		margin-left: auto;
		margin-right: auto;
	}

	.hero-actions {
		margin-top: 40px;
	}

	.download-button {
		display: inline-block;
		background: white;
		color: #667eea;
		padding: 16px 40px;
		border-radius: 12px;
		font-size: 1.2rem;
		font-weight: 600;
		text-decoration: none;
		transition: transform 0.2s ease, box-shadow 0.2s ease;
		box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
	}

	.download-button:hover {
		transform: translateY(-2px);
		box-shadow: 0 6px 20px rgba(0, 0, 0, 0.3);
	}

	.download-button:active {
		transform: translateY(0);
	}

	/* Screenshot Section */
	.screenshot-section {
		padding: 100px 0;
		background: white;
		margin-top: -40px;
		position: relative;
		z-index: 1;
	}

	.screenshot-container {
		max-width: 1400px;
		margin: 0 auto;
		text-align: center;
	}

	.screenshot-title {
		font-size: 2.5rem;
		font-weight: 700;
		margin: 0 0 20px;
		color: #333;
		letter-spacing: -0.01em;
	}

	.screenshot-subtitle {
		font-size: 1.2rem;
		margin: 0 0 50px;
		color: #666;
	}

	.screenshot-wrapper {
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 0;
		width: 100%;
	}

	.screenshot {
		width: 100%;
		height: auto;
		display: block;
	}

	/* Features Section */
	.features {
		padding: 100px 0;
		background: #f8f9fa;
		border-radius: 40px 40px 0 0;
		margin-top: -40px;
		position: relative;
		z-index: 0;
	}

	.section-title {
		font-size: 2.5rem;
		font-weight: 700;
		text-align: center;
		margin: 0 0 60px;
		color: #333;
		letter-spacing: -0.01em;
	}

	.features-grid {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 20px;
		margin-top: 40px;
		max-width: 600px;
		margin-left: auto;
		margin-right: auto;
	}

	.feature-card {
		background: #f8f9fa;
		border-radius: 20px;
		padding: 30px 40px;
		text-align: center;
		transition: transform 0.3s ease, box-shadow 0.3s ease;
		border: 1px solid #e9ecef;
		width: 100%;
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: flex-start;
		gap: 30px;
	}

	.feature-card-content {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		text-align: left;
		flex: 1;
	}

	.feature-card:hover {
		transform: translateY(-8px);
		box-shadow: 0 12px 40px rgba(0, 0, 0, 0.1);
	}

	.feature-icon {
		font-size: 3rem;
		flex-shrink: 0;
	}

	.feature-title {
		font-size: 1.5rem;
		font-weight: 600;
		margin: 0 0 8px;
		color: #333;
	}

	.feature-description {
		font-size: 1rem;
		color: #666;
		margin: 0;
		line-height: 1.6;
	}

	/* Footer */
	.footer {
		background: #1a1a1a;
		color: white;
		padding: 60px 0 40px;
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
		margin-bottom: 30px;
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

	.contact {
		padding-top: 30px;
		border-top: 1px solid #333;
	}

	.contact-title {
		font-size: 1.3rem;
		font-weight: 600;
		margin: 0 0 20px;
		color: white;
	}

	.contact-info {
		font-size: 1rem;
		color: #ccc;
		margin: 0;
	}

	.contact-info a {
		color: #667eea;
		text-decoration: none;
		transition: color 0.3s ease;
	}

	.contact-info a:hover {
		color: #764ba2;
		text-decoration: underline;
	}

	/* Responsive Design */
	@media (max-width: 768px) {
		.title {
			font-size: 2.5rem;
		}

		.subtitle {
			font-size: 1.2rem;
		}

		.description {
			font-size: 1rem;
		}

		.download-button {
			padding: 14px 30px;
			font-size: 1.1rem;
		}

		.features {
			padding: 60px 0;
		}

		.section-title {
			font-size: 2rem;
		}

		.features-grid {
			max-width: 100%;
			padding: 0 10px;
		}

		.feature-card {
			flex-direction: column;
			text-align: center;
			padding: 30px 25px;
			gap: 20px;
		}

		.feature-card-content {
			align-items: center;
			text-align: center;
		}

		.hero {
			padding: 60px 0 80px;
		}

		.screenshot-section {
			padding: 60px 0;
		}

		.screenshot-title {
			font-size: 2rem;
		}

		.screenshot-subtitle {
			font-size: 1rem;
		}

		.features {
			border-radius: 30px 30px 0 0;
		}

		.screenshot-wrapper {
			padding: 0 10px;
		}
	}
</style>
