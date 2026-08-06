# index.html-2
Data recovery
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Recovery Guru | Local HDD, SSD & RAID Data Recovery Specialists</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#f0fdf4',
                            500: '#22c55e',
                            600: '#16a34a',
                            700: '#15803d',
                            accent: '#a3e635',
                            dark: '#0b0f19',
                            card: '#151c2c',
                            border: '#2a3447'
                        }
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-brand-dark text-slate-100 font-sans antialiased selection:bg-brand-500 selection:text-black">

    <!-- 1. TOP ANNOUNCEMENT BANNER -->
    <div class="bg-gradient-to-r from-brand-600 via-emerald-600 to-teal-600 text-white text-xs md:text-sm py-2 px-4 text-center font-medium shadow-md">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between gap-2">
            <span><i class="fa-solid fa-truck-pickup mr-2"></i> Onsite pick-up service available in Greater Boston & Providence area for just $20!</span>
            <button onclick="openModal()" class="underline font-bold hover:text-brand-accent transition">Request Pickup & Diagnosis &rarr;</button>
        </div>
    </div>

    <!-- 2. STICKY HEADER & NAVIGATION -->
    <header class="sticky top-0 z-40 bg-brand-dark/95 backdrop-blur border-b border-brand-border">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <!-- Logo -->
                <a href="#" class="flex items-center gap-3">
                    <div class="w-10 h-10 bg-brand-500 rounded-xl flex items-center justify-center text-black font-extrabold text-xl shadow-lg shadow-brand-500/20">
                        <i class="fa-solid fa-database"></i>
                    </div>
                    <div>
                        <span class="text-xl font-black tracking-tight text-white block">DATA RECOVERY <span class="text-brand-500">GURU</span></span>
                        <span class="text-[10px] tracking-widest uppercase text-slate-400 block font-semibold">Local Lab & Cleanroom Service</span>
                    </div>
                </a>

                <!-- Desktop Navigation -->
                <nav class="hidden lg:flex items-center space-x-6 text-sm font-medium text-slate-300">
                    <a href="#services" class="hover:text-brand-500 transition">Services</a>
                    <a href="#process" class="hover:text-brand-500 transition">10-Step Process</a>
                    <a href="#locations" class="hover:text-brand-500 transition">Locations</a>
                    <a href="#reviews" class="hover:text-brand-500 transition">Reviews</a>
                    <a href="#faq" class="hover:text-brand-500 transition">Why Us</a>
                </nav>

                <!-- Action Buttons -->
                <div class="hidden sm:flex items-center gap-3">
                    <a href="tel:6175719172" class="flex items-center gap-2 bg-brand-card hover:bg-slate-800 text-slate-200 border border-brand-border px-4 py-2.5 rounded-lg text-sm font-semibold transition">
                        <i class="fa-solid fa-phone text-brand-500"></i> (617) 571-9172
                    </a>
                    <button onclick="openModal()" class="bg-brand-500 hover:bg-brand-600 text-black font-bold px-5 py-2.5 rounded-lg text-sm shadow-lg shadow-brand-500/25 transition">
                        Free Diagnosis
                    </button>
                </div>

                <!-- Mobile Menu Toggle Button -->
                <button onclick="toggleMobileMenu()" class="lg:hidden p-2 text-slate-300 hover:text-white">
                    <i class="fa-solid fa-bars text-2xl" id="menuIcon"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Menu Dropdown -->
        <div id="mobileMenu" class="hidden lg:hidden bg-brand-card border-b border-brand-border px-4 pt-2 pb-6 space-y-3">
            <a href="#services" onclick="toggleMobileMenu()" class="block py-2 text-slate-200 hover:text-brand-500 font-medium">Services & Devices</a>
            <a href="#process" onclick="toggleMobileMenu()" class="block py-2 text-slate-200 hover:text-brand-500 font-medium">10-Step Process</a>
            <a href="#locations" onclick="toggleMobileMenu()" class="block py-2 text-slate-200 hover:text-brand-500 font-medium">Lab Locations</a>
            <a href="#reviews" onclick="toggleMobileMenu()" class="block py-2 text-slate-200 hover:text-brand-500 font-medium">Reviews</a>
            <div class="pt-4 border-t border-brand-border flex flex-col gap-3">
                <a href="tel:6175719172" class="w-full text-center bg-slate-800 text-white py-3 rounded-lg font-bold border border-brand-border">
                    <i class="fa-solid fa-phone text-brand-500 mr-2"></i> Call (617) 571-9172
                </a>
                <button onclick="openModal(); toggleMobileMenu();" class="w-full bg-brand-500 text-black py-3 rounded-lg font-bold">
                    Get Free Diagnosis
                </button>
            </div>
        </div>
    </header>

    <!-- 3. HERO SECTION -->
    <section class="relative py-16 lg:py-24 overflow-hidden border-b border-brand-border">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid lg:grid-cols-12 gap-12 items-center">
                
                <!-- Hero Left Content -->
                <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                    <div class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-brand-500/10 border border-brand-500/30 text-brand-500 text-xs font-bold tracking-wide uppercase">
                        <span class="w-2 h-2 rounded-full bg-brand-500 animate-pulse"></span>
                        Local Lab • Cleanroom Equipped • Talk Directly To An Engineer
                    </div>
                    
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight text-white leading-tight">
                        Local Data Recovery Specialists in <span class="text-transparent bg-clip-text bg-gradient-to-r from-brand-500 to-brand-accent">Boston & Providence</span>
                    </h1>
                    
                    <p class="text-lg text-slate-300 max-w-2xl mx-auto lg:mx-0 leading-relaxed">
                        No recovery, no charge policy. Full transparency, zero hidden fees, and rapid local diagnostic evaluation. Talk directly to senior technicians—not high-pressure salespeople.
                    </p>

                    <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-2">
                        <button onclick="openModal()" class="w-full sm:w-auto bg-brand-500 hover:bg-brand-600 text-black font-extrabold text-base px-8 py-4 rounded-xl shadow-xl shadow-brand-500/20 transition flex items-center justify-center gap-2">
                            <span>Get Started With Free Diagnosis</span>
                            <i class="fa-solid fa-arrow-right"></i>
                        </button>
                        
                        <a href="tel:6175719172" class="w-full sm:w-auto bg-brand-card hover:bg-slate-800 text-white font-bold text-base px-6 py-4 rounded-xl border border-brand-border transition flex items-center justify-center gap-2">
                            <i class="fa-solid fa-phone text-brand-500"></i>
                            <span>Call/Text (617) 571-9172</span>
                        </a>
                    </div>

                    <!-- Trust Badges -->
                    <div class="pt-6 grid grid-cols-2 sm:grid-cols-4 gap-4 border-t border-brand-border/60 text-slate-400 text-xs font-medium">
                        <div class="flex items-center gap-2"><i class="fa-solid fa-shield-halved text-brand-500 text-base"></i> ISO 5 Cleanroom</div>
                        <div class="flex items-center gap-2"><i class="fa-solid fa-handshake text-brand-500 text-base"></i> No Recovery - No Fee</div>
                        <div class="flex items-center gap-2"><i class="fa-solid fa-bolt text-brand-500 text-base"></i> Onsite Pickup Option</div>
                        <div class="flex items-center gap-2"><i class="fa-solid fa-star text-brand-500 text-base"></i> 5-Star Rated Lab</div>
                    </div>
                </div>

                <!-- Hero Right - Quick Service Form -->
                <div class="lg:col-span-5">
                    <div class="bg-brand-card border border-brand-border rounded-2xl p-6 sm:p-8 shadow-2xl relative">
                        <h3 class="text-xl font-bold text-white mb-2">Request Instant Evaluation</h3>
                        <p class="text-xs text-slate-400 mb-6">Receive a clear quote and recovery guidance within minutes.</p>

                        <form onsubmit="handleQuickForm(event)" class="space-y-4">
                            <div>
                                <label class="block text-xs font-semibold text-slate-300 uppercase mb-1">Your Full Name</label>
                                <input type="text" required placeholder="John Doe" class="w-full bg-slate-900 border border-slate-700 rounded-lg px-4 py-2.5 text-slate-100 text-sm focus:outline-none focus:border-brand-500">
                            </div>

                            <div>
                                <label class="block text-xs font-semibold text-slate-300 uppercase mb-1">Phone / WhatsApp</label>
                                <input type="tel" required placeholder="(617) 000-0000" class="w-full bg-slate-900 border border-slate-700 rounded-lg px-4 py-2.5 text-slate-100 text-sm focus:outline-none focus:border-brand-500">
                            </div>

                            <div>
                                <label class="block text-xs font-semibold text-slate-300 uppercase mb-1">Device Type</label>
                                <select class="w-full bg-slate-900 border border-slate-700 rounded-lg px-4 py-2.5 text-slate-100 text-sm focus:outline-none focus:border-brand-500">
                                    <option>External Hard Drive (HDD)</option>
                                    <option>Solid State Drive (SSD / NVMe)</option>
                                    <option>RAID Array / NAS Server</option>
                                    <option>MacBook / Laptop Disk</option>
                                    <option>USB Flash Drive / SD Card</option>
                                </select>
                            </div>

                            <div>
                                <label class="block text-xs font-semibold text-slate-300 uppercase mb-1">Issue Description</label>
                                <textarea rows="3" placeholder="Describe symptoms (clicking noise, not mounting, accidental format...)" class="w-full bg-slate-900 border border-slate-700 rounded-lg px-4 py-2.5 text-slate-100 text-sm focus:outline-none focus:border-brand-500"></textarea>
                            </div>

                            <button type="submit" class="w-full bg-brand-500 hover:bg-brand-600 text-black font-extrabold py-3.5 rounded-lg transition text-sm shadow-md">
                                Submit For Free Technical Review &rarr;
                            </button>
                        </form>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- 4. LOCATION TICKER -->
    <div class="bg-slate-900/80 border-b border-brand-border py-4 overflow-hidden">
        <div class="max-w-7xl mx-auto px-4 flex flex-wrap justify-center items-center gap-6 text-xs text-slate-400 font-semibold uppercase tracking-wider">
            <span><i class="fa-solid fa-location-dot text-brand-500 mr-1.5"></i> Boston, MA</span>
            <span>•</span>
            <span><i class="fa-solid fa-location-dot text-brand-500 mr-1.5"></i> Cambridge (Harvard Sq)</span>
            <span>•</span>
            <span><i class="fa-solid fa-location-dot text-brand-500 mr-1.5"></i> Dedham, MA</span>
            <span>•</span>
            <span><i class="fa-solid fa-location-dot text-brand-500 mr-1.5"></i> Burlington</span>
            <span>•</span>
            <span><i class="fa-solid fa-location-dot text-brand-500 mr-1.5"></i> Framingham</span>
            <span>•</span>
            <span><i class="fa-solid fa-location-dot text-brand-500 mr-1.5"></i> Providence, RI</span>
            <span>•</span>
            <span><i class="fa-solid fa-location-dot text-brand-500 mr-1.5"></i> Nashua, NH</span>
        </div>
    </div>

    <!-- 5. 3-STEP WORKFLOW OVERVIEW -->
    <section class="py-16 bg-brand-dark border-b border-brand-border">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-12">
                <h2 class="text-3xl font-extrabold text-white">Simple 3-Step Recovery Workflow</h2>
                <p class="text-slate-400 text-sm mt-2">How we safely diagnostic, extract, and return your critical files.</p>
            </div>

            <div class="grid md:grid-cols-3 gap-8 relative">
                <!-- Step 1 -->
                <div class="bg-brand-card border border-brand-border rounded-2xl p-8 relative hover:border-brand-500/50 transition">
                    <div class="w-12 h-12 bg-brand-500/20 text-brand-500 rounded-xl flex items-center justify-center font-extrabold text-xl mb-6">1</div>
                    <h3 class="text-xl font-bold text-white mb-2">Free Diagnosis</h3>
                    <p class="text-sm text-slate-300 leading-relaxed">Drop off, ship in, or schedule a $20 local technician pickup. We test the drive in our cleanroom and provide a guaranteed quote.</p>
                </div>

                <!-- Step 2 -->
                <div class="bg-brand-card border border-brand-border rounded-2xl p-8 relative hover:border-brand-500/50 transition">
                    <div class="w-12 h-12 bg-brand-500/20 text-brand-500 rounded-xl flex items-center justify-center font-extrabold text-xl mb-6">2</div>
                    <h3 class="text-xl font-bold text-white mb-2">Data Extraction</h3>
                    <p class="text-sm text-slate-300 leading-relaxed">Our engineers repair hardware, fix firmware, clone magnetic platters using hardware image tools, and extract your raw data.</p>
                </div>

                <!-- Step 3 -->
                <div class="bg-brand-card border border-brand-border rounded-2xl p-8 relative hover:border-brand-500/50 transition">
                    <div class="w-12 h-12 bg-brand-500/20 text-brand-500 rounded-xl flex items-center justify-center font-extrabold text-xl mb-6">3</div>
                    <h3 class="text-xl font-bold text-white mb-2">Review & Delivery</h3>
                    <p class="text-sm text-slate-300 leading-relaxed">You review the full target file directory before making any payment. Upon approval, data is delivered on a target drive or cloud storage.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 6. 10-STEP PROCESS INTERACTIVE ACCORDION -->
    <section id="process" class="py-20 bg-slate-900 border-b border-brand-border">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <span class="text-brand-500 text-xs font-bold uppercase tracking-widest">Full Transparency</span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-white mt-1">Our Complete 10-Step Recovery Process</h2>
                <p class="text-slate-400 text-sm mt-2">Click any step below to see how our engineering lab safely handles your drive.</p>
            </div>

            <div class="space-y-3" id="accordionContainer">
                <!-- Step items injected/rendered via structured markup -->
                <script>
                    const steps = [
                        { title: "1. Request Free Diagnostic Evaluation", content: "Contact our lab via telephone, message, or online modal. We gather hardware symptoms and advise immediate steps to prevent permanent platter damage." },
                        { title: "2. Flexible Intake (Drop-Off, Ship-In, or $20 Pickup)", content: "Choose between dropping off at one of our 6 regional offices, shipping directly to our main lab, or letting an engineer pick up the device at your door." },
                        { title: "3. Cleanroom & Hardware Diagnostics", content: "Engineers inspect drive electronics, heads, PCB firmware, and read/write heads inside an ISO 5 cleanroom using PC-3000 diagnostic systems." },
                        { title: "4. Written Diagnostic Report & Flat Rate Quote", content: "You receive a technical assessment explaining hardware or logical failures alongside a firm, no-obligation repair quote." },
                        { title: "5. Customer Service Approval", content: "No work proceeds without your explicit go-ahead. If you choose not to proceed, you pay nothing for the diagnosis." },
                        { title: "6. Mechanical Stabilisation & Sector-Level Cloning", content: "We perform micro-soldering, head replacements, or firmware patches, creating a sector-by-sector binary clone to avoid stress on original media." },
                        { title: "7. File System Reconstruction & Data Extraction", content: "Advanced software algorithms extract raw structures, rebuilding file indexes, photo libraries, databases, and document folders." },
                        { title: "8. File List Verification Prior to Payment", content: "We send you a verified directory file list. You inspect the recovered filenames and tree structure before paying a single cent." },
                        { title: "9. Payment Execution & Secure Media Handover", content: "Upon satisfaction, complete payment via Zelle, credit card, check, or corporate PO. Recovered data is placed on a fresh encrypted drive." },
                        { title: "10. 10-Day Warranty & Secure Disposal Options", content: "We maintain a encrypted mirror backup for 10 days to verify seamless restoration on your home or office computers." }
                    ];
                </script>
            </div>
        </div>
    </section>

    <!-- 7. SERVICES & STORAGE DEVICES GRID -->
    <section id="services" class="py-20 bg-brand-dark border-b border-brand-border">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl sm:text-4xl font-extrabold text-white">Devices & Media We Service</h2>
                <p class="text-slate-400 text-sm mt-2">Comprehensive mechanical, electrical, and file system recovery across all formats.</p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Hard Drive -->
                <div class="bg-brand-card border border-brand-border rounded-xl p-6 hover:border-brand-500 transition">
                    <i class="fa-solid fa-hard-drive text-3xl text-brand-500 mb-4"></i>
                    <h3 class="text-lg font-bold text-white mb-2">Hard Disk Drives (HDD)</h3>
                    <ul class="text-xs text-slate-300 space-y-2">
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Click of Death / Beeping drives</li>
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Motor & spindle failures</li>
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Head assembly replacement</li>
                    </ul>
                </div>

                <!-- SSD / NVMe -->
                <div class="bg-brand-card border border-brand-border rounded-xl p-6 hover:border-brand-500 transition">
                    <i class="fa-solid fa-microchip text-3xl text-brand-500 mb-4"></i>
                    <h3 class="text-lg font-bold text-white mb-2">Solid State Drives (SSD)</h3>
                    <ul class="text-xs text-slate-300 space-y-2">
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Controller chip failures</li>
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Unrecognized NVMe / M.2</li>
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> NAND chip off-board extraction</li>
                    </ul>
                </div>

                <!-- RAID & Servers -->
                <div class="bg-brand-card border border-brand-border rounded-xl p-6 hover:border-brand-500 transition">
                    <i class="fa-solid fa-server text-3xl text-brand-500 mb-4"></i>
                    <h3 class="text-lg font-bold text-white mb-2">RAID & NAS Arrays</h3>
                    <ul class="text-xs text-slate-300 space-y-2">
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> RAID 0, 1, 5, 6, 10 recovery</li>
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Synology, QNAP, Promise Pegasus</li>
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Re-building missing parities</li>
                    </ul>
                </div>

                <!-- Flash & Flash Drives -->
                <div class="bg-brand-card border border-brand-border rounded-xl p-6 hover:border-brand-500 transition">
                    <i class="fa-solid fa-memory text-3xl text-brand-500 mb-4"></i>
                    <h3 class="text-lg font-bold text-white mb-2">USB & Flash Cards</h3>
                    <ul class="text-xs text-slate-300 space-y-2">
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Broken USB connector repairs</li>
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Corrupted SD & MicroSD media</li>
                        <li><i class="fa-solid fa-check text-brand-500 mr-1.5"></i> Monolith chip trace soldering</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- 8. REGIONAL LOCATIONS -->
    <section id="locations" class="py-20 bg-slate-900 border-b border-brand-border">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-12">
                <h2 class="text-3xl font-extrabold text-white">Greater Boston Lab Offices</h2>
                <p class="text-slate-400 text-sm mt-2">Visit one of our convenient regional drop-off centers or lab headquarters.</p>
            </div>

            <div class="grid md:grid-cols-3 gap-8">
                <!-- Location 1 -->
                <div class="bg-brand-card border border-brand-border rounded-xl p-6">
                    <div class="text-brand-500 text-xl font-bold mb-1"><i class="fa-solid fa-building mr-2"></i> Boston Back Bay</div>
                    <p class="text-slate-300 text-xs mb-4">100 Massachusetts Ave., Suite 500<br>Boston, MA 02115</p>
                    <div class="text-xs text-slate-400 space-y-1">
                        <div><strong>Hours:</strong> Mon - Fri: 9:00 AM - 4:30 PM</div>
                        <div><strong>Phone:</strong> (617) 571-9172</div>
                    </div>
                </div>

                <!-- Location 2 -->
                <div class="bg-brand-card border border-brand-border rounded-xl p-6">
                    <div class="text-brand-500 text-xl font-bold mb-1"><i class="fa-solid fa-building mr-2"></i> Cambridge Harvard Sq.</div>
                    <p class="text-slate-300 text-xs mb-4">1 Mifflin Place, Suite 400<br>Cambridge, MA 02138</p>
                    <div class="text-xs text-slate-400 space-y-1">
                        <div><strong>Hours:</strong> Mon - Fri: 9:00 AM - 4:30 PM</div>
                        <div><strong>Phone:</strong> (617) 571-9172</div>
                    </div>
                </div>

                <!-- Location 3 -->
                <div class="bg-brand-card border border-brand-border rounded-xl p-6">
                    <div class="text-brand-500 text-xl font-bold mb-1"><i class="fa-solid fa-building mr-2"></i> Dedham Office</div>
                    <p class="text-slate-300 text-xs mb-4">3 Allied Dr., Suite 303<br>Dedham, MA 02026</p>
                    <div class="text-xs text-slate-400 space-y-1">
                        <div><strong>Hours:</strong> Mon - Fri: 9:00 AM - 4:30 PM</div>
                        <div><strong>Phone:</strong> (617) 571-9172</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 9. REVIEWS CAROUSEL / GRID -->
    <section id="reviews" class="py-20 bg-brand-dark border-b border-brand-border">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-12">
                <span class="text-brand-500 text-xs font-bold uppercase tracking-widest">Verified Feedback</span>
                <h2 class="text-3xl font-extrabold text-white mt-1">What Our Clients Say</h2>
            </div>

            <div class="grid md:grid-cols-3 gap-6">
                <div class="bg-brand-card border border-brand-border p-6 rounded-xl flex flex-col justify-between">
                    <p class="text-xs text-slate-300 leading-relaxed italic">"Stop looking - you want to go to these guys! Prompt, professional service at a great price. They're local, which is a massive plus. Saved all our business files!"</p>
                    <div class="mt-4 pt-4 border-t border-brand-border flex items-center justify-between">
                        <span class="text-xs font-bold text-white">— BJ MacLaughlin</span>
                        <div class="text-amber-400 text-xs"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></div>
                    </div>
                </div>

                <div class="bg-brand-card border border-brand-border p-6 rounded-xl flex flex-col justify-between">
                    <p class="text-xs text-slate-300 leading-relaxed italic">"Petri gave us his personal attention and recovered all over 20 years of business data. Service is outstanding and Petri is of the highest integrity."</p>
                    <div class="mt-4 pt-4 border-t border-brand-border flex items-center justify-between">
                        <span class="text-xs font-bold text-white">— Bill Murray</span>
                        <div class="text-amber-400 text-xs"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></div>
                    </div>
                </div>

                <div class="bg-brand-card border border-brand-border p-6 rounded-xl flex flex-col justify-between">
                    <p class="text-xs text-slate-300 leading-relaxed italic">"Knock-me-on-my-ass impressed with them! They over-deliver well before the deadline and at a price you won't find anywhere else."</p>
                    <div class="mt-4 pt-4 border-t border-brand-border flex items-center justify-between">
                        <span class="text-xs font-bold text-white">— Eric Carpenter</span>
                        <div class="text-amber-400 text-xs"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 10. FOOTER -->
    <footer class="bg-slate-950 text-slate-400 text-xs py-12 border-t border-brand-border pb-24 sm:pb-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-4 gap-8 mb-8">
                <div>
                    <span class="text-lg font-bold text-white block mb-3">DATA RECOVERY <span class="text-brand-500">GURU</span></span>
                    <p class="text-slate-400 leading-relaxed">Local hard drive, solid state drive, and RAID array data recovery laboratory serving Massachusetts and Rhode Island.</p>
                </div>
                <div>
                    <h4 class="text-white font-bold mb-3">Quick Navigation</h4>
                    <ul class="space-y-2">
                        <li><a href="#services" class="hover:text-brand-500">HDD & SSD Recovery</a></li>
                        <li><a href="#services" class="hover:text-brand-500">RAID Array Reconstruct</a></li>
                        <li><a href="#process" class="hover:text-brand-500">Diagnostic Process</a></li>
                        <li><a href="#locations" class="hover:text-brand-500">Boston & Cambridge Offices</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-white font-bold mb-3">Contact Direct</h4>
                    <p class="mb-1 text-slate-300">Hotline: (617) 571-9172</p>
                    <p class="mb-1">Channels: Call, Text, WhatsApp, Signal</p>
                    <p class="text-slate-400">Emergency 24/7 Intake Available</p>
                </div>
                <div>
                    <h4 class="text-white font-bold mb-3">Guarantee</h4>
                    <p class="text-slate-400 leading-relaxed">No Recovery - No Charge policy applies to all hardware and mechanical fault recoveries.</p>
                </div>
            </div>

            <div class="pt-8 border-t border-slate-800 text-center text-slate-500">
                <p>&copy; 2015-2026 Data Recovery Guru. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- 11. MOBILE PERSISTENT CALL BAR -->
    <div class="fixed bottom-0 inset-x-0 bg-brand-dark/95 border-t border-brand-border p-3 flex sm:hidden gap-2 z-30 backdrop-blur">
        <a href="tel:6175719172" class="flex-1 bg-slate-800 text-white font-bold py-3 text-center rounded-lg text-xs flex items-center justify-center gap-1.5 border border-brand-border">
            <i class="fa-solid fa-phone text-brand-500"></i> Call / Text
        </a>
        <button onclick="openModal()" class="flex-1 bg-brand-500 text-black font-extrabold py-3 text-center rounded-lg text-xs shadow-lg">
            Free Diagnosis
        </button>
    </div>

    <!-- 12. FREE DIAGNOSIS MODAL POPUP -->
    <div id="diagnosisModal" class="fixed inset-0 bg-black/80 backdrop-blur-sm z-50 hidden flex items-center justify-center p-4">
        <div class="bg-brand-card border border-brand-border rounded-2xl max-w-lg w-full p-6 sm:p-8 relative shadow-2xl">
            <button onclick="closeModal()" class="absolute top-4 right-4 text-slate-400 hover:text-white text-xl">
                <i class="fa-solid fa-xmark"></i>
            </button>

            <h3 class="text-2xl font-black text-white mb-1">Start Free Diagnosis</h3>
            <p class="text-xs text-slate-400 mb-6">No obligation. An engineer will evaluate your case immediately.</p>

            <form onsubmit="handleModalSubmit(event)" class="space-y-4">
                <div>
                    <label class="block text-xs font-semibold text-slate-300 uppercase mb-1">Full Name</label>
                    <input type="text" required placeholder="Jane Smith" class="w-full bg-slate-900 border border-slate-700 rounded-lg px-4 py-2 text-slate-100 text-sm focus:outline-none focus:border-brand-500">
                </div>

                <div>
                    <label class="block text-xs font-semibold text-slate-300 uppercase mb-1">Phone Number</label>
                    <input type="tel" required placeholder="(617) 571-9172" class="w-full bg-slate-900 border border-slate-700 rounded-lg px-4 py-2 text-slate-100 text-sm focus:outline-none focus:border-brand-500">
                </div>

                <div>
                    <label class="block text-xs font-semibold text-slate-300 uppercase mb-1">Delivery Method</label>
                    <select class="w-full bg-slate-900 border border-slate-700 rounded-lg px-4 py-2 text-slate-100 text-sm focus:outline-none focus:border-brand-500">
                        <option>Drop-Off At Office (Boston, Cambridge, Dedham)</option>
                        <option>Request Onsite Tech Pickup ($20)</option>
                        <option>Mail-In / Ship Drive</option>
                    </select>
                </div>

                <div>
                    <label class="block text-xs font-semibold text-slate-300 uppercase mb-1">Describe Drive Problem</label>
                    <textarea rows="3" placeholder="Drive fell down, stopped turning on, clicking sound..." class="w-full bg-slate-900 border border-slate-700 rounded-lg px-4 py-2 text-slate-100 text-sm focus:outline-none focus:border-brand-500"></textarea>
                </div>

                <button type="submit" class="w-full bg-brand-500 hover:bg-brand-600 text-black font-extrabold py-3.5 rounded-lg transition text-sm">
                    Submit Request
                </button>
            </form>
        </div>
    </div>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        // Render 10-Step Process Accordion
        const container = document.getElementById('accordionContainer');
        steps.forEach((step, idx) => {
            const item = document.createElement('div');
            item.className = 'bg-brand-card border border-brand-border rounded-xl overflow-hidden';
            item.innerHTML = `
                <button onclick="toggleAccordion(${idx})" class="w-full p-4 text-left flex justify-between items-center text-slate-100 font-bold text-sm hover:text-brand-500 transition">
                    <span>${step.title}</span>
                    <i class="fa-solid fa-chevron-down text-xs text-slate-400 transition-transform duration-200" id="icon-${idx}"></i>
                </button>
                <div id="content-${idx}" class="hidden p-4 pt-0 text-xs text-slate-300 leading-relaxed border-t border-brand-border/40">
                    ${step.content}
                </div>
            `;
            container.appendChild(item);
        });

        function toggleAccordion(index) {
            const content = document.getElementById(`content-${index}`);
            const icon = document.getElementById(`icon-${index}`);
            const isHidden = content.classList.contains('hidden');
            
            if (isHidden) {
                content.classList.remove('hidden');
                icon.classList.add('rotate-180');
            } else {
                content.classList.add('hidden');
                icon.classList.remove('rotate-180');
            }
        }

        // Mobile Menu Toggle
        function toggleMobileMenu() {
            const menu = document.getElementById('mobileMenu');
            menu.classList.toggle('hidden');
        }

        // Modal Open/Close
        function openModal() {
            document.getElementById('diagnosisModal').classList.remove('hidden');
        }

        function closeModal() {
            document.getElementById('diagnosisModal').classList.add('hidden');
        }

        // Form Submission Stubs
        function handleQuickForm(e) {
            e.preventDefault();
            alert('Thank you! Your request has been logged. A senior data recovery engineer will contact you shortly.');
        }

        function handleModalSubmit(e) {
            e.preventDefault();
            alert('Free diagnosis request submitted successfully! Our team will reach out via call/text.');
            closeModal();
        }
    </script>
</body>
</html>
