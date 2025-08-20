# Jack-landing-page-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Property Network - Hands-Off Property Investment</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html, body {
            overflow-x: hidden;
        }
        
        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #2c3e50;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .container {
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        
        .hero {
            background: white;
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            margin-bottom: 40px;
            text-align: center;
            position: relative;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: -5px;
            left: -5px;
            right: -5px;
            bottom: -5px;
            background: linear-gradient(45deg, #f093fb 0%, #f5576c 25%, #4facfe 50%, #00f2fe 100%);
            border-radius: 25px;
            z-index: -1;
            animation: borderGlow 3s ease-in-out infinite alternate;
        }
        
        @keyframes borderGlow {
            0% { opacity: 0.7; }
            100% { opacity: 1; }
        }
        
        .preheader {
            background: #e74c3c;
            color: white;
            padding: 8px 20px;
            border-radius: 25px;
            display: inline-block;
            font-size: 14px;
            font-weight: bold;
            margin-bottom: 20px;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        h1 {
            font-size: 2.5em;
            color: #2c3e50;
            margin-bottom: 20px;
            line-height: 1.2;
        }
        
        .subheader {
            font-size: 1.3em;
            color: #34495e;
            margin-bottom: 30px;
        }
        
        .vsl-container {
            margin: 30px 0;
            position: relative;
        }
        
        .vsl-icon {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 40px 30px;
            border-radius: 15px;
            cursor: pointer;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            text-align: center;
            text-decoration: none;
            display: block;
        }
        
        .vsl-icon:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }
        
        .play-button {
            width: 80px;
            height: 80px;
            background: rgba(255,255,255,0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            position: relative;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .play-button::after {
            content: '';
            width: 0;
            height: 0;
            border-left: 25px solid #2c3e50;
            border-top: 15px solid transparent;
            border-bottom: 15px solid transparent;
            margin-left: 8px;
        }
        
        .vsl-text {
            color: white;
            font-size: 1.2em;
            font-weight: bold;
            line-height: 1.3;
        }
        
        .cta-button {
            background: linear-gradient(135deg, #ff6b6b 0%, #ee5a24 100%);
            color: white;
            padding: 18px 40px;
            border: none;
            border-radius: 50px;
            font-size: 1.2em;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
            margin-top: 20px;
            box-shadow: 0 10px 20px rgba(238, 90, 36, 0.3);
        }
        
        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 30px rgba(238, 90, 36, 0.4);
        }
        
        .section {
            background: white;
            margin-bottom: 40px;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        h2 {
            font-size: 2em;
            margin-bottom: 25px;
            color: #2c3e50;
            text-align: center;
        }
        
        h3 {
            font-size: 1.5em;
            margin-bottom: 15px;
            color: #e74c3c;
        }
        
        p {
            margin-bottom: 20px;
            font-size: 1.1em;
            line-height: 1.7;
        }
        
        .highlight {
            background: linear-gradient(120deg, #ffeaa7 0%, #fab1a0 100%);
            padding: 3px 8px;
            border-radius: 5px;
            font-weight: bold;
        }
        
        .bullet-points {
            list-style: none;
            padding: 0;
        }
        
        .bullet-points li {
            margin-bottom: 15px;
            padding-left: 30px;
            position: relative;
            font-size: 1.1em;
        }
        
        .bullet-points li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #27ae60;
            font-weight: bold;
            font-size: 1.2em;
        }
        
        .testimonial {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            padding: 25px;
            border-radius: 15px;
            margin: 20px 0;
            color: white;
            position: relative;
        }
        
        .testimonial::before {
            content: '"';
            font-size: 4em;
            position: absolute;
            top: -10px;
            left: 20px;
            opacity: 0.3;
        }
        
        .urgency-box {
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 100%);
            padding: 20px;
            border-radius: 10px;
            border-left: 5px solid #e74c3c;
            margin: 20px 0;
        }
        
        .faq-item {
            margin-bottom: 25px;
            padding-bottom: 25px;
            border-bottom: 1px solid #ecf0f1;
        }
        
        .faq-question {
            font-weight: bold;
            font-size: 1.2em;
            margin-bottom: 10px;
            color: #2c3e50;
        }
        
        @media (max-width: 1024px) {
            .container {
                padding: 15px;
            }
            
            h1 {
                font-size: 2em;
            }
            
            .hero {
                padding: 30px;
            }
            
            .section {
                padding: 30px;
            }
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 1.8em;
            }
            
            .subheader {
                font-size: 1.1em;
            }
            
            .hero {
                padding: 20px;
            }
            
            .section {
                padding: 20px;
            }
            
            .play-button {
                width: 60px;
                height: 60px;
            }
            
            .play-button::after {
                border-left: 20px solid #2c3e50;
                border-top: 12px solid transparent;
                border-bottom: 12px solid transparent;
            }
            
            .cta-button {
                padding: 15px 30px;
                font-size: 1.1em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- HERO SECTION -->
        <div class="hero">
            <div class="preheader">Attention: Busy UK Professionals & Entrepreneurs</div>
            <h1>Build A £100K+ Property Portfolio In 12 Months Without Dealing With Tenants, Repairs, Or Hunting For Deals</h1>
            <div class="subheader">Finally... get the passive income you want without becoming a full-time landlord, learning complex property laws, or risking your money on dodgy deals</div>
            
            <div class="vsl-container">
                <a href="https://docs.google.com/document/d/1KPwP6BRAWW-rn-ayzhjhYlMK136dfErKvRGYUYWMGi4/edit?usp=sharing" class="vsl-icon">
                    <div class="play-button"></div>
                    <div class="vsl-text">Click Here To See The: VSL I WROTE FOR YOU</div>
                </a>
            </div>
            
            <a href="#" class="cta-button">Book Your Property Strategy Call Now</a>
        </div>

        <!-- PROBLEM IDENTIFICATION -->
        <div class="section">
            <h2>You're Tired Of Watching Everyone Else Build Wealth While You Stay Stuck</h2>
            
            <p>You've seen the headlines...</p>
            
            <p>Property prices climbing 8-12% per year in Manchester hotspots.</p>
            
            <p>Your mates bragging about their £2,000+ monthly rental income.</p>
            
            <p>Yet here you are... still on the sidelines.</p>
            
            <p><strong>You've tried the "traditional" route:</strong></p>
            
            <p>Spent hours trawling Rightmove and Zoopla looking for deals that don't exist...</p>
            
            <p>Called letting agents who couldn't care less about your investment goals...</p>
            
            <p>Read property books that gave you theory but zero practical help...</p>
            
            <p>Maybe you even bought a course that left you more confused than when you started.</p>
            
            <p>And the worst part?</p>
            
            <p><span class="highlight">Every month you wait, property prices climb further out of reach while your savings lose value to inflation.</span></p>
            
            <p>You're stuck in analysis paralysis while other investors are building generational wealth.</p>
            
            <p>But what if I told you there's a completely different way?</p>
            
            <p>A way that doesn't require you to become a property expert overnight...</p>
            
            <p>Or spend your weekends driving around looking at run-down houses...</p>
            
            <p>Or dealing with 2 AM phone calls about broken boilers...</p>
        </div>

        <!-- ORIGIN STORY -->
        <div class="section">
            <h2>How A £47,000 Mistake Led To The Most Profitable Property System In The UK</h2>
            
            <p><em>[INSERT FOUNDER NAME AND PHOTO HERE]</em></p>
            
            <p>Three years ago, I was exactly where you are now.</p>
            
            <p>Successful in my corporate job, but watching my money sit in savings accounts earning nothing while property prices soared.</p>
            
            <p>I decided to "do it myself."</p>
            
            <p>Big mistake.</p>
            
            <p>I bought what I thought was a "bargain" - a Victorian terrace in Manchester for £120K.</p>
            
            <p>The surveyor missed the structural issues. The renovation went £25K over budget. The first tenant trashed the place and disappeared without paying rent.</p>
            
            <p>Total loss: <span class="highlight">£47,000</span> and eight months of pure stress.</p>
            
            <p>I was ready to give up on property completely...</p>
            
            <p>Until I met someone at a networking event who changed everything.</p>
            
            <p>He owned 23 properties across the North West. All profitable. All managed.</p>
            
            <p>But here's the kicker - he'd never renovated a single one himself.</p>
            
            <p>Never dealt with a tenant directly.</p>
            
            <p>Never even viewed most of the properties before buying them.</p>
            
            <p>"I don't invest in property," he told me. "I invest in <strong>systems.</strong>"</p>
            
            <p>That's when I realized why 90% of property investors fail...</p>
            
            <p>They're trying to do everything themselves instead of leveraging proven systems and expertise.</p>
            
            <p>They're working IN their property business instead of ON it.</p>
            
            <p>I spent the next 18 months building the system that became The Property Network...</p>
            
            <p>And now our clients are getting results like these:</p>
            
            <div class="testimonial">
                <p><em>[INSERT CLIENT TESTIMONIAL WITH SPECIFIC RESULTS HERE]</em></p>
                <p><strong>- Client Name, Location</strong></p>
            </div>
        </div>

        <!-- SOLUTION REVELATION -->
        <div class="section">
            <h2>The "Done-For-You" Property System That's Creating Millionaires</h2>
            
            <p>Here's what separates The Property Network from every other property company...</p>
            
            <p>We don't just find you deals.</p>
            
            <p>We don't just manage your properties.</p>
            
            <p>We build you a complete, profitable property business from A to Z.</p>
            
            <p><strong>Here's exactly how it works:</strong></p>
            
            <h3>Phase 1: Intelligence & Strategy</h3>
            <p>We analyze the market data you'll never see. House price trends, rental demand, upcoming infrastructure projects, demographic shifts. We identify the exact postcodes where your money will work hardest.</p>
            
            <h3>Phase 2: Sourcing & Acquisition</h3>
            <p>Our team sources properties before they hit the market. We negotiate below asking price, handle all the legal work, and present you with complete investment packages - not random properties.</p>
            
            <h3>Phase 3: Renovation & Optimization</h3>
            <p>Our trusted contractors handle every aspect of renovation. From planning permission to final touches. You get progress photos, but you never have to visit a building site or argue with a tradesman.</p>
            
            <h3>Phase 4: Tenant Management</h3>
            <p>We find and vet tenants using our 12-point screening process. Handle all the paperwork, deposits, and legal compliance. Your property is cash-flowing from day one.</p>
            
            <p><strong>The result?</strong></p>
            
            <p>You wake up to rental payments in your bank account without lifting a finger.</p>
            
            <p>Your property values climb while you focus on your career.</p>
            
            <p>You build real wealth without becoming a full-time landlord.</p>
            
            <ul class="bullet-points">
                <li><strong>Property Investment Playbook:</strong> Get the exact strategies we use to identify 15%+ ROI deals → Sleep peacefully knowing you're building wealth while others guess → Become the investor who always finds opportunities</li>
                
                <li><strong>Bespoke Deal Sourcing:</strong> We hunt down off-market properties that fit your exact criteria → Skip the stress of property viewings and negotiations → Become the investor with access to the best deals</li>
                
                <li><strong>Complete Project Management:</strong> From planning to completion, we handle everything → Enjoy your weekends instead of dealing with contractors → Become the hands-off investor you always wanted to be</li>
                
                <li><strong>Professional Tenant Management:</strong> We screen, manage, and handle all tenant issues → Never deal with late-night emergency calls again → Become the landlord who earns without the drama</li>
                
                <li><strong>Legal & Compliance Management:</strong> We handle all regulations, safety certificates, and legal requirements → Sleep soundly knowing you're protected from legislation changes → Become the investor who's always compliant</li>
            </ul>
            
            <div class="testimonial">
                <p><em>[INSERT BEFORE/AFTER CLIENT STORY WITH SPECIFIC NUMBERS HERE]</em></p>
                <p><strong>- Client Name, Portfolio Value</strong></p>
            </div>
        </div>

        <!-- PRODUCT INTRODUCTION -->
        <div class="section">
            <h2>Introducing: The Complete Property Wealth System</h2>
            
            <p>Everything you need to build a profitable property portfolio without becoming a full-time landlord.</p>
            
            <p><strong>What You Get:</strong></p>
            
            <h3>The Property Investment Playbook</h3>
            <ul class="bullet-points">
                <li>Property investment fundamentals course</li>
                <li>Tax and accounting strategies</li>
                <li>Hotspot identification guides</li>
                <li>ROI calculators and analysis tools</li>
                <li>Step-by-step walkthrough videos</li>
                <li>Quick-reference cheat sheets</li>
            </ul>
            
            <h3>Bespoke Property Sourcing Service</h3>
            <ul class="bullet-points">
                <li>One-on-one strategy consultation</li>
                <li>Custom property search based on your budget and goals</li>
                <li>Off-market deal access</li>
                <li>Complete financial analysis for each property</li>
                <li>Negotiation and purchase support</li>
            </ul>
            
            <h3>Full Project Management</h3>
            <ul class="bullet-points">
                <li>Trusted contractor network</li>
                <li>Complete renovation management</li>
                <li>Weekly progress updates</li>
                <li>Quality control and final inspections</li>
                <li>Move-in ready property delivery</li>
            </ul>
            
            <h3>Ongoing Property Management</h3>
            <ul class="bullet-points">
                <li>Professional tenant screening</li>
                <li>Rent collection and financial reporting</li>
                <li>Maintenance and repair coordination</li>
                <li>Legal compliance management</li>
                <li>Performance monitoring and optimization</li>
            </ul>
            
            <h3>Exclusive Support & Community</h3>
            <ul class="bullet-points">
                <li>Private WhatsApp support group</li>
                <li>Monthly group coaching calls</li>
                <li>Email and phone support</li>
                <li>Market updates and opportunities</li>
                <li>Access to exclusive deals</li>
            </ul>
            
            <p>Compare this to hiring separate agents, project managers, and property managers...</p>
            
            <p>You'd pay £5,000+ in fees and still lack the coordination and expertise we provide.</p>
            
            <p>Our clients typically see returns that justify the investment within the first property deal.</p>
        </div>

        <!-- OFFER STRUCTURE -->
        <div class="section">
            <h2>Your Investment In Financial Freedom</h2>
            
            <p>The Property Investment Playbook alone would cost you £2,000 if you bought similar courses separately.</p>
            
            <p>Professional property sourcing services charge £3,000-£5,000 per deal.</p>
            
            <p>Project management typically runs 10-15% of renovation costs.</p>
            
            <p>And ongoing property management fees are usually 8-12% of rental income.</p>
            
            <p>But because our system is so efficient, we can offer everything at a fraction of what it would cost separately.</p>
            
            <div class="urgency-box">
                <p><strong>Book Your Strategy Call Today</strong></p>
                <p>We're limiting new clients to 10 per month to ensure quality service. Only 3 spots remain for this month.</p>
            </div>
            
            <p><strong>Our Guarantee:</strong></p>
            
            <p>If we don't identify at least 3 profitable deal opportunities in your first 90 days, we'll work with you free until we do.</p>
            
            <a href="#" class="cta-button">Book Your Strategy Call Before Spots Fill</a>
        </div>

        <!-- FAQ SECTION -->
        <div class="section">
            <h2>Questions Smart Investors Ask</h2>
            
            <div class="faq-item">
                <div class="faq-question">Q: How much money do I need to get started?</div>
                <p>Most of our clients start with £25K-£50K as a deposit, but we work with budgets from £15K upwards. During your strategy call, we'll discuss financing options including bridging loans and joint ventures that can multiply your buying power.</p>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: What if I don't know anything about property investment?</div>
                <p>Perfect. Our system works best with beginners because you won't have bad habits to break. The Playbook teaches you everything you need to know, and our team handles the complex stuff. You'll become educated without the expensive mistakes.</p>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: How long before I see returns?</div>
                <p>Most properties are generating rental income within 3-6 months of purchase. Your first property should cover your investment in our system within 12-18 months through rental income and capital appreciation.</p>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: What if the property market crashes?</div>
                <p>We focus on areas with strong rental demand and limited supply. Even in downturns, people need places to live. Our properties are selected for consistent rental income, not just capital growth. Plus, we teach you strategies to profit in any market condition.</p>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: How is this different from other property investment companies?</div>
                <p>Most companies either sell you courses with no implementation support, or they're agents who just find properties. We provide complete end-to-end service - education, sourcing, renovation, and management. You get a business, not just properties.</p>
            </div>
            
            <p>Still have questions? Let's talk on your strategy call.</p>
            
            <p>Because while you're reading this...</p>
            
            <p>Someone else is booking their call and taking the last spot.</p>
            
            <p>Property prices won't wait for you to "think about it."</p>
            
            <p>Your financial freedom won't build itself.</p>
            
            <a href="#" class="cta-button">Book Your Strategy Call Now - Only 3 Spots Left</a>
        </div>
    </div>
</body>
</html>
