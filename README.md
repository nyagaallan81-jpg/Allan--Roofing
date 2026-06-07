Here is the complete, responsive HTML and CSS code for the Allan Roofing landing page. It is designed as a single-page template that you can save and open directly in your browser.
The contact buttons are pre-configured to launch a phone call or open a WhatsApp chat immediately when clicked on a mobile device.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Allan Roofing | Expert Roofing Solutions in Nairobi</title>
    <style>
        /* Base Styles */
        :root {
            --primary-color: #1A365D; /* Trustworthy Dark Blue */
            --secondary-color: #E53E3E; /* Action-oriented Red */
            --whatsapp-color: #25D366; /* Official WhatsApp Green */
            --text-color: #333;
            --bg-light: #F7FAFC;
        }
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            color: var(--text-color);
            line-height: 1.6;
        }
        h1, h2, h3 {
            margin-top: 0;
            color: var(--primary-color);
        }
        a {
            text-decoration: none;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Buttons */
        .btn {
            display: inline-block;
            padding: 12px 24px;
            color: white;
            border-radius: 5px;
            font-weight: bold;
            text-align: center;
            transition: opacity 0.3s ease;
        }
        .btn:hover {
            opacity: 0.9;
        }
        .btn-call {
            background-color: var(--secondary-color);
        }
        .btn-whatsapp {
            background-color: var(--whatsapp-color);
        }
        
        /* Header */
        header {
            background-color: white;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        .logo {
            font-size: 24px;
            font-weight: 900;
            color: var(--primary-color);
        }
        
        /* Hero Section */
        .hero {
            background-color: var(--primary-color);
            color: white;
            padding: 80px 20px;
            text-align: center;
        }
        .hero h1 {
            color: white;
            font-size: 40px;
            margin-bottom: 20px;
        }
        .hero p {
            font-size: 18px;
            max-width: 600px;
            margin: 0 auto 30px auto;
        }
        .hero-buttons {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        /* Trust & Services Sections */
        .section {
            padding: 60px 20px;
        }
        .bg-gray {
            background-color: var(--bg-light);
        }
        .section-header {
            text-align: center;
            margin-bottom: 40px;
        }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }
        .card {
            background: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            text-align: center;
        }
        
        /* Testimonials */
        .testimonial {
            font-style: italic;
            border-left: 4px solid var(--secondary-color);
            padding-left: 15px;
            margin-bottom: 20px;
            background: white;
            padding: 20px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }
        
        /* Final CTA */
        .cta-section {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 60px 20px;
        }
        .cta-section h2 {
            color: white;
        }
        
        /* Footer */
        footer {
            background-color: #112240;
            color: white;
            text-align: center;
            padding: 30px 20px;
        }
        
        /* Mobile Adjustments */
        @media (max-width: 600px) {
            .hero h1 {
                font-size: 32px;
            }
            .header-content {
                flex-direction: column;
                gap: 15px;
            }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <div class="header-content">
            <div class="logo">Allan Roofing</div>
            <a href="tel:0742180988" class="btn btn-call">Free Quote: 0742180988</a>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Expert Roofing Solutions You Can Trust in Nairobi.</h1>
            <p>Protect your property with top-quality materials and unmatched craftsmanship. From emergency leak repairs to complete roof installations, we get the job done right.</p>
            <div class="hero-buttons">
                <!-- Using +254 for Kenyan WhatsApp link formatting -->
                <a href="https://wa.me/254117227729" target="_blank" class="btn btn-whatsapp">Chat on WhatsApp</a>
                <a href="tel:0742180988" class="btn btn-call">Call Us Now</a>
            </div>
        </div>
    </section>

    <!-- Trust Section -->
    <section class="section bg-gray">
        <div class="container">
            <div class="section-header">
                <h2>Why Choose Allan Roofing?</h2>
            </div>
            <div class="grid">
                <div class="card">
                    <h3>Rapid Response</h3>
                    <p>We understand that roofing emergencies cannot wait. We are just a quick call or message away.</p>
                </div>
                <div class="card">
                    <h3>Quality Craftsmanship</h3>
                    <p>We use highly durable, weather-resistant materials designed specifically to stand the test of time.</p>
                </div>
                <div class="card">
                    <h3>Honest Pricing</h3>
                    <p>No hidden fees. You receive a clear, transparent, and upfront quote before any work begins.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="section">
        <div class="container">
            <div class="section-header">
                <h2>Comprehensive Roofing Services</h2>
            </div>
            <div class="grid">
                <div class="card">
                    <h3>Leak Detection & Repair</h3>
                    <p>Fast and effective solutions to find the source of the problem and stop water damage in its tracks.</p>
                </div>
                <div class="card">
                    <h3>New Roof Installations</h3>
                    <p>Professional, secure, and beautiful installations for both residential and commercial properties.</p>
                </div>
                <div class="card">
                    <h3>Roof Maintenance</h3>
                    <p>Regular inspections and preventative upkeep to maximize the lifespan of your roof.</p>
                </div>
                <div class="card">
                    <h3>Gutter Services</h3>
                    <p>Seamless installation, deep cleaning, and repair for proper water drainage away from your foundation.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Social Proof Section -->
    <section class="section bg-gray">
        <div class="container">
            <div class="section-header">
                <h2>What Our Clients Say</h2>
            </div>
            <div class="grid" style="grid-template-columns: 1fr 1fr;">
                <div class="testimonial">
                    <p>"Allan Roofing responded quickly to my emergency leak. Professional, clean, and reasonably priced."</p>
                    <strong>– Happy Customer, Nairobi</strong>
                </div>
                <div class="testimonial">
                    <p>"Excellent job on our new roof. The team was efficient and the final result looks fantastic. Highly recommend."</p>
                    <strong>– Satisfied Homeowner</strong>
                </div>
            </div>
        </div>
    </section>

    <!-- Final Call to Action -->
    <section class="cta-section">
        <div class="container">
            <h2>Ready to Secure Your Roof?</h2>
            <p style="margin-bottom: 30px;">Reach out today for a free inspection and quote. Let the experts handle it.</p>
            <div class="hero-buttons">
                <a href="https://wa.me/254117227729" target="_blank" class="btn btn-whatsapp">Message Us (0117227729)</a>
                <a href="tel:0742180988" class="btn btn-call">Call 0742180988</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <h3>Allan Roofing</h3>
            <p>Serving Nairobi and surrounding regions.</p>
            <p>Contact: <a href="tel:0742180988" style="color: #E53E3E;">0742180988</a> | <a href="https://wa.me/254117227729" style="color: #25D366;">0117227729</a></p>
            <p style="margin-top: 20px; font-size: 14px; opacity: 0.7;">&copy; 2026 Allan Roofing. All rights reserved.</p>
        </div>
    </footer>

</body>
</html>

```
# Allan--Roofing
A roofing company trusted by many
