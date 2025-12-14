<script>
	import logo from '$lib/assets/logo.png';
</script>

<svelte:head>
	<title>Privacy Policy - MindChips</title>
	<meta name="description" content="MindChips Privacy Policy - Your privacy matters to us. Learn how we protect your data and ensure your information stays secure." />
</svelte:head>

<div class="container">
	<!-- Header Section -->
	<section class="header">
		<div class="header-content">
			<img src={logo} alt="MindChips Logo" class="logo" />
			<h1 class="title">Your Privacy Matters to Us</h1>
			<p class="subtitle">At MindChips, we are committed to protecting your privacy and ensuring the security of your personal information.</p>
		</div>
	</section>

	<!-- Content Section -->
	<section class="content">
		<div class="content-wrapper">
			<p class="intro">
				We understand that privacy is a fundamental right, and we have designed our application with your privacy as a top priority. This privacy policy explains how we handle your data and what you can expect when using MindChips.
			</p>

			<div class="section">
				<h2 class="section-title">No Data Collection</h2>
				<p class="section-text">
					MindChips operates entirely on your local device. We do not collect, store, or transmit any personal information, usage data, or analytics. Specifically:
				</p>
				<ul class="list">
					<li>No personal information is collected or stored</li>
					<li>No usage analytics or tracking data is gathered</li>
					<li>No application logs or diagnostic information is transmitted</li>
					<li>No user preferences or settings are sent to external servers</li>
					<li>All application data remains on your local machine</li>
				</ul>
				<p class="section-text">
					Everything you do with MindChips stays on your device. We have no servers, no databases, and no way to access your information even if we wanted to.
				</p>
			</div>

			<div class="section">
				<h2 class="section-title">No Data Sharing</h2>
				<p class="section-text">
					Since we do not collect any data, there is nothing to share. MindChips does not:
				</p>
				<ul class="list">
					<li>Share data with third parties</li>
					<li>Sell user information to advertisers or data brokers</li>
					<li>Use third-party analytics services</li>
					<li>Integrate with advertising networks</li>
					<li>Participate in any data sharing agreements</li>
				</ul>
				<p class="section-text">
					Your privacy is protected by design. There is no data pipeline, no network requests, and no external communication beyond what is necessary for the application to function on your Mac.
				</p>
			</div>

			<div class="section">
				<h2 class="section-title">Legal Compliance</h2>
				<p class="section-text">
					MindChips is designed to comply with major privacy regulations, including:
				</p>
				<ul class="list">
					<li>
						<strong>GDPR (General Data Protection Regulation):</strong> As we do not collect or process personal data, MindChips naturally complies with GDPR requirements.
					</li>
					<li>
						<strong>CCPA (California Consumer Privacy Act):</strong> Since no personal information is collected, there is no data to disclose, delete, or opt-out of.
					</li>
					<li>
						<strong>PIPEDA (Personal Information Protection and Electronic Documents Act):</strong> Our zero-data-collection approach ensures compliance with Canadian privacy laws.
					</li>
				</ul>
				<p class="section-text">
					If you have any questions about our compliance with specific privacy regulations, please feel free to contact us using the information provided below.
				</p>
			</div>

			<div class="section">
				<h2 class="section-title">Contact Information</h2>
				<p class="section-text">
					If you have any questions, concerns, or requests regarding this privacy policy or how MindChips handles your information, please contact us:
				</p>
				<p class="contact-info">
					Email: <a href="mailto:pochonlee@gmail.com">pochonlee@gmail.com</a>
				</p>
				<p class="section-text">
					We will respond to your inquiries as soon as possible, typically within 48 hours.
				</p>
			</div>

			<div class="last-updated">
				<p>Last updated: Dec 30, 2025</p>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="footer">
		<div class="footer-content">
			<p class="footer-text">© 2025 Scrapmind.com All rights reserved.</p>
			<div class="footer-links">
				<a href="/" class="footer-link">Home</a>
				<span class="separator">|</span>
				<a href="/privacy" class="footer-link">Privacy Policy</a>
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

	/* Content Section */
	.content {
		background: white;
		border-radius: 30px 30px 0 0;
		margin-top: -40px;
		position: relative;
		z-index: 1;
		padding: 60px 40px;
		min-height: calc(100vh - 300px);
	}

	.content-wrapper {
		max-width: 800px;
		margin: 0 auto;
	}

	.intro {
		font-size: 1.1rem;
		line-height: 1.8;
		color: #555;
		margin: 0 0 40px;
	}

	.section {
		margin-bottom: 50px;
	}

	.section-title {
		font-size: 2rem;
		font-weight: 700;
		margin: 0 0 20px;
		color: #333;
		letter-spacing: -0.01em;
	}

	.section-text {
		font-size: 1rem;
		line-height: 1.8;
		color: #555;
		margin: 0 0 15px;
	}

	.list {
		margin: 20px 0;
		padding-left: 30px;
		color: #555;
	}

	.list li {
		font-size: 1rem;
		line-height: 1.8;
		margin-bottom: 12px;
	}

	.list li strong {
		color: #333;
		font-weight: 600;
	}

	.contact-info {
		font-size: 1.1rem;
		margin: 20px 0;
		padding: 20px;
		background: #f8f9fa;
		border-radius: 10px;
		border-left: 4px solid #667eea;
	}

	.contact-info a {
		color: #667eea;
		text-decoration: none;
		font-weight: 500;
		transition: color 0.3s ease;
	}

	.contact-info a:hover {
		color: #764ba2;
		text-decoration: underline;
	}

	.last-updated {
		margin-top: 50px;
		padding-top: 30px;
		border-top: 1px solid #e9ecef;
		text-align: center;
	}

	.last-updated p {
		font-size: 0.9rem;
		color: #999;
		margin: 0;
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

		.content {
			padding: 40px 20px;
		}

		.section-title {
			font-size: 1.6rem;
		}

		.intro {
			font-size: 1rem;
		}

		.section-text {
			font-size: 0.95rem;
		}

		.list {
			padding-left: 20px;
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

