<script lang="ts">
	import { onMount } from 'svelte';

    // Foundation partners
    const partners = [
        { name: 'Ford Foundation' },
        { name: 'Rockefeller Foundation' },
        { name: 'Gates Foundation' },
        { name: 'MacArthur Foundation' },
        { name: 'Kresge Foundation' },
        { name: 'Knight Foundation' },
        { name: 'Lumina Foundation' },
        { name: 'Hewlett Foundation' },
        { name: 'Packard Foundation' },
        { name: 'Carnegie Corporation' },
        { name: 'Mellon Foundation' },
        { name: 'Open Society Foundations' },
        { name: 'Walton Family Foundation' },
        { name: 'Robert Wood Johnson Foundation' }
    ];

    const articles = [
        {
            tag: 'Case Study',
            title: 'How Knight Foundation Streamlined Grant Review',
            desc: 'Reduced application review time by 60% while improving scoring consistency across program officers.',
            img: '/generated/image-foundation-executive-reviewing-reports-o-1766298472458-3.webp',
            bg: 'bg-primary-50'
        },
        {
            tag: 'Research',
            title: 'The Cost of Inconsistent Grant Scoring',
            desc: 'New research reveals how subjective evaluation criteria lead to missed opportunities and inequitable funding.',
            img: '/generated/image-diverse-team-of-foundation-staff-collabo-1766298468141-1.webp',
            bg: 'bg-gray-50'
        },
        {
            tag: 'Guide',
            title: 'Automated Grantee Reporting: Best Practices',
            desc: 'Learn how leading foundations use AI to track performance and reduce administrative burden on grantees.',
            img: '/generated/image-professional-foundation-program-officer--1766298465592-0.webp',
            bg: 'bg-primary-50'
        },
        {
            tag: 'Insights',
            title: 'The Future of Philanthropic Due Diligence',
            desc: 'How automation and AI are transforming the way foundations evaluate impact and allocate resources.',
            img: '/generated/image-foundation-executive-reviewing-reports-o-1766298472458-3.webp',
            bg: 'bg-gray-50'
        }
    ];

    const testimonials = [
        {
            quote: "GrantScope transformed our review process. We now score 200+ applications consistently in half the time, and our automated reporting gives us real-time visibility into grantee performance.",
            author: "Sarah Mitchell",
            role: "Senior Program Officer",
            company: "Regional Community Foundation",
            img: "/generated/image-confident-female-foundation-program-offi-1766298470318-2.webp"
        }
    ];
</script>

<div class="min-h-screen bg-white text-gray-900 font-sans selection:bg-gray-200">
    <!-- Header -->
    <header class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-sm border-b border-gray-100">
        <div class="max-w-[1600px] mx-auto px-6 py-6 flex justify-between items-center">
            <div class="w-64">
                <a href="/" class="text-xl font-semibold tracking-tight text-gray-900">
                    GrantScope
                </a>
            </div>
            <div>
                <a href="#" class="bg-gray-900 text-white px-5 py-2.5 text-xs font-medium rounded-sm hover:bg-gray-800 transition-colors">
                    Request a Demo
                </a>
            </div>
        </div>
    </header>

    <main class="pt-32 pb-20">
        <div class="max-w-[1600px] mx-auto px-6 grid grid-cols-12 gap-8">
            <!-- Sidebar Navigation -->
            <div class="col-span-2 hidden lg:block sticky top-32 h-fit">
                <nav class="flex flex-col space-y-3 text-xs text-gray-500 font-medium">
                    <a href="#" class="text-gray-900">Home</a>
                    <a href="#" class="hover:text-gray-900 transition-colors">Product</a>
                    <a href="#" class="hover:text-gray-900 transition-colors">How It Works</a>
                    <a href="#" class="hover:text-gray-900 transition-colors">Resources</a>
                    <a href="#" class="hover:text-gray-900 transition-colors">About</a>
                </nav>
            </div>

            <!-- Main Content Area -->
            <div class="col-span-12 lg:col-span-10 space-y-32">
                
                <!-- Hero Section -->
                <section class="relative">
                    <div class="relative w-full h-[600px] overflow-hidden rounded-sm">
                        <!-- Hero Background Image -->
                        <img src="/generated/image-professional-foundation-program-officer--1766298465592-0.webp" alt="Foundation program officer reviewing grants" class="absolute inset-0 w-full h-full object-cover" />
                        <div class="absolute inset-0 bg-gradient-to-r from-white/95 via-white/85 to-transparent"></div>
                        
                        <div class="absolute inset-0 flex flex-col items-center justify-center p-12 text-center">
                            <h1 class="text-4xl md:text-5xl font-normal text-gray-900 mb-6 max-w-3xl leading-tight">
                                AI-powered grant scoring and automated grantee reporting for foundations
                            </h1>
                            <p class="text-lg text-gray-600 mb-12 max-w-2xl">
                                Score applications consistently against custom criteria, then track performance through automated report analysis
                            </p>

                            <!-- Logos Card -->
                            <div class="bg-white/95 backdrop-blur-sm p-8 rounded-sm shadow-sm max-w-4xl w-full">
                                <p class="text-[10px] text-gray-500 mb-6 uppercase tracking-wide">
                                    Trusted by leading foundations managing over $15B in annual grants
                                </p>
                                <div class="grid grid-cols-3 md:grid-cols-7 gap-8 items-center justify-items-center opacity-70">
                                    {#each partners.slice(0, 14) as partner}
                                        <div class="h-6 flex items-center justify-center">
                                            <span class="text-[10px] font-semibold text-gray-700">{partner.name}</span>
                                        </div>
                                    {/each}
                                </div>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- How GrantScope Works Section -->
                <section>
                    <div class="flex justify-between items-baseline mb-24 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900 max-w-xl leading-tight">
                            How GrantScope transforms grant management
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Our Platform</span>
                    </div>

                    <div class="relative min-h-[800px]">
                        <!-- Diagram -->
                        <div class="absolute right-0 top-0 w-1/2 p-8 bg-gray-50 rounded-sm">
                            <div class="text-[10px] text-gray-500 mb-4 uppercase tracking-wide">Automated Workflow</div>
                            <div class="flex items-center justify-between gap-4">
                                <div class="w-32 h-32 bg-gray-900 text-white flex flex-col items-center justify-center p-4 rounded-sm">
                                    <div class="mb-2">
                                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg>
                                    </div>
                                    <span class="text-[10px] uppercase tracking-wider text-center">Grant Applications</span>
                                </div>
                                
                                <div class="flex-1 h-32 bg-primary-50 border border-primary-200 rounded-sm flex flex-col items-center justify-center relative">
                                    <span class="text-[10px] text-gray-500 uppercase absolute top-2 left-4">AI Scoring</span>
                                    <div class="w-full border-t border-dashed border-gray-300 absolute top-1/2"></div>
                                    
                                    <!-- Score Icon -->
                                    <div class="absolute -bottom-6 bg-white border border-gray-200 p-2 shadow-sm rounded-sm flex items-center gap-2">
                                        <div class="w-8 h-10 border border-primary-300 flex items-center justify-center bg-primary-50">
                                            <div class="text-xs font-bold text-primary-700">95</div>
                                        </div>
                                        <div class="text-[8px] leading-tight text-gray-500">
                                            CONSISTENT<br>SCORING
                                        </div>
                                    </div>
                                </div>

                                <div class="w-32 h-32 bg-gradient-to-br from-primary-600 to-primary-700 text-white flex flex-col items-center justify-center p-4 rounded-sm">
                                    <div class="mb-2">
                                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z"></path></svg>
                                    </div>
                                    <span class="text-[10px] uppercase tracking-wider text-center">Performance Tracking</span>
                                </div>
                            </div>
                        </div>

                        <!-- Text Blocks -->
                        <div class="absolute left-0 top-[200px] max-w-md">
                            <div class="flex gap-4">
                                <span class="bg-gray-900 text-white w-5 h-5 flex items-center justify-center text-xs font-medium shrink-0 rounded-sm">1</span>
                                <p class="text-sm text-gray-600 leading-relaxed">
                                    <strong class="text-gray-900">AI-Powered Scoring:</strong> Applications are automatically evaluated against your custom criteria, ensuring consistent scoring across all program officers and eliminating subjective bias.
                                </p>
                            </div>
                        </div>

                        <div class="absolute left-0 top-[400px] max-w-md">
                            <div class="flex gap-4">
                                <span class="bg-gray-900 text-white w-5 h-5 flex items-center justify-center text-xs font-medium shrink-0 rounded-sm">2</span>
                                <p class="text-sm text-gray-600 leading-relaxed">
                                    <strong class="text-gray-900">Automated Diligence:</strong> Our platform analyzes financial documents, organizational capacity, and track records to surface key insights for faster, more informed decision-making.
                                </p>
                            </div>
                        </div>

                        <div class="absolute left-0 top-[600px] max-w-md">
                            <div class="flex gap-4">
                                <span class="bg-gray-900 text-white w-5 h-5 flex items-center justify-center text-xs font-medium shrink-0 rounded-sm">3</span>
                                <p class="text-sm text-gray-600 leading-relaxed">
                                    <strong class="text-gray-900">Performance Monitoring:</strong> Track grantee progress through automated report analysis, giving you real-time visibility into outcomes and impact without manual data entry.
                                </p>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- Why GrantScope Section -->
                <section>
                    <div class="flex justify-between items-baseline mb-16 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900">
                            Built for the future of philanthropy
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Our Mission</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-3 gap-12 text-sm leading-relaxed text-gray-600 mb-24">
                        <p>
                            GrantScope is transforming how foundations manage their $15 billion philanthropy portfolio through AI-powered automation.
                        </p>
                        <div class="space-y-6">
                            <p>
                                Foundation program officers face an impossible challenge: review hundreds of grant applications with limited time and resources, while maintaining consistent evaluation standards and tracking grantee performance across diverse portfolios.
                            </p>
                            <p>
                                Manual review processes lead to inconsistent scoring, missed opportunities, and administrative burden that prevents foundations from focusing on what matters most—maximizing social impact.
                            </p>
                        </div>
                        <div class="space-y-6">
                            <p>
                                GrantScope automates the entire grant lifecycle, from application scoring to performance monitoring. Our AI analyzes applications against your custom criteria, ensuring every proposal receives fair, consistent evaluation. Automated report analysis gives you real-time insights into grantee outcomes.
                            </p>
                            <p>
                                We're helping foundations scale their impact by reducing review time by 60%, improving scoring consistency, and enabling data-driven decisions that maximize the effectiveness of every dollar granted.
                            </p>
                        </div>
                    </div>

                    <!-- Featured In -->
                    <div class="bg-gray-50 rounded-sm p-8 flex items-center justify-between">
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider mr-8">As featured in:</span>
                        <div class="flex-1 flex justify-between items-center opacity-60">
                            <span class="font-serif text-xl font-bold">The Chronicle of Philanthropy</span>
                            <span class="font-sans text-lg font-semibold">Stanford Social Innovation Review</span>
                            <span class="font-serif text-lg">Inside Philanthropy</span>
                            <span class="font-serif text-lg">Nonprofit Quarterly</span>
                        </div>
                    </div>
                </section>

                <!-- Key Features Dark Section -->
                <section class="bg-gray-950 text-white rounded-sm overflow-hidden relative min-h-[400px] flex items-center">
                    <!-- Background Graphic -->
                    <div class="absolute inset-0 opacity-20">
                        <div class="absolute bottom-0 left-0 right-0 h-64 bg-gradient-to-t from-primary-900/30 to-transparent"></div>
                        <!-- Abstract pattern -->
                        <svg class="absolute bottom-0 w-full h-full text-primary-900/20" viewBox="0 0 100 100" preserveAspectRatio="none">
                            <path d="M0 100 Q 50 50 100 100" fill="none" stroke="currentColor" stroke-width="0.5" />
                            <path d="M0 100 Q 50 40 100 100" fill="none" stroke="currentColor" stroke-width="0.5" />
                            <path d="M0 100 Q 50 30 100 100" fill="none" stroke="currentColor" stroke-width="0.5" />
                        </svg>
                    </div>

                    <div class="relative z-10 p-16 w-full grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                        <div>
                            <h2 class="text-3xl font-light mb-6">
                                Scale from pilot to 100K grants<br>with automated workflows
                            </h2>
                            <p class="text-sm text-gray-400 mb-8 max-w-md">
                                Our platform handles custom scoring criteria, multi-stage review processes, and automated performance tracking—all while integrating seamlessly with your existing grant management systems.
                            </p>
                            <button class="bg-white text-gray-900 px-6 py-2 text-xs font-medium rounded-sm hover:bg-gray-200 transition-colors">
                                See How It Works
                            </button>
                        </div>
                        <div class="flex justify-end">
                            <div class="grid grid-cols-2 gap-4">
                                <div class="bg-white/10 backdrop-blur-sm border border-white/20 rounded-sm p-6 flex flex-col items-center justify-center text-center">
                                    <div class="text-3xl font-bold text-white mb-2">60%</div>
                                    <div class="text-[10px] uppercase tracking-wider text-gray-400">Faster Review</div>
                                </div>
                                <div class="bg-white/10 backdrop-blur-sm border border-white/20 rounded-sm p-6 flex flex-col items-center justify-center text-center">
                                    <div class="text-3xl font-bold text-white mb-2">100K</div>
                                    <div class="text-[10px] uppercase tracking-wider text-gray-400">Grants Tracked</div>
                                </div>
                                <div class="bg-white/10 backdrop-blur-sm border border-white/20 rounded-sm p-6 flex flex-col items-center justify-center text-center">
                                    <div class="text-3xl font-bold text-white mb-2">95%</div>
                                    <div class="text-[10px] uppercase tracking-wider text-gray-400">Score Consistency</div>
                                </div>
                                <div class="bg-white/10 backdrop-blur-sm border border-white/20 rounded-sm p-6 flex flex-col items-center justify-center text-center">
                                    <div class="text-3xl font-bold text-white mb-2">$15B</div>
                                    <div class="text-[10px] uppercase tracking-wider text-gray-400">Grants Managed</div>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- Testimonials -->
                <section>
                    <div class="flex justify-between items-baseline mb-16 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900">
                            Trusted by foundation leaders
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Testimonials</span>
                    </div>

                    <div class="relative">
                        <div class="flex gap-8 overflow-hidden">
                            <div class="w-full md:w-[800px] shrink-0 bg-gray-50 flex">
                                <div class="w-1/3 shrink-0">
                                    <img src="/generated/image-confident-female-foundation-program-offi-1766298470318-2.webp" alt="Sarah Mitchell" class="w-full h-full object-cover" />
                                </div>
                                <div class="w-2/3 p-12 flex flex-col justify-center">
                                    <blockquote class="text-xl font-light leading-relaxed mb-8">
                                        "GrantScope transformed our review process. We now score 200+ applications consistently in half the time, and our automated reporting gives us real-time visibility into grantee performance."
                                    </blockquote>
                                    <div class="flex items-center gap-2 mb-3">
                                        <div class="w-6 h-6 bg-primary-500 rounded-sm flex items-center justify-center">
                                            <span class="text-[10px] font-bold text-white">RCF</span>
                                        </div>
                                        <span class="text-xs font-semibold text-gray-600">Regional Community Foundation</span>
                                    </div>
                                    <div>
                                        <div class="font-medium text-gray-900">Sarah Mitchell</div>
                                        <div class="text-xs text-gray-500">Senior Program Officer</div>
                                    </div>
                                </div>
                            </div>
                            <!-- Next slide preview -->
                            <div class="w-1/3 shrink-0 opacity-50">
                                <img src="/generated/image-diverse-team-of-foundation-staff-collabo-1766298468141-1.webp" alt="Next testimonial" class="w-full h-full object-cover" />
                            </div>
                        </div>
                        
                        <!-- Navigation Button -->
                        <button class="absolute top-0 right-0 -mt-12 w-8 h-8 bg-gray-900 text-white flex items-center justify-center hover:bg-gray-800 rounded-sm">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path></svg>
                        </button>
                    </div>
                </section>

                <!-- Read More / Articles -->
                <section>
                    <div class="flex justify-between items-baseline mb-16 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900">
                            Read more
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Articles</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                        {#each articles as article}
                            <div class="group cursor-pointer">
                                <div class="relative aspect-square mb-6 overflow-hidden {article.bg} flex items-center justify-center">
                                    <span class="absolute top-4 left-4 text-[10px] uppercase tracking-wider bg-white/50 px-2 py-1 backdrop-blur-sm">{article.tag}</span>
                                    <!-- Use text overlay instead of image if image fails, but styling div with bg color -->
                                    <div class="text-center p-4">
                                        <!-- Placeholder graphic -->
                                        <div class="text-2xl font-serif italic opacity-50">{article.title.split(' ')[0]}</div>
                                    </div>
                                </div>
                                <h3 class="text-lg font-normal mb-3 leading-tight group-hover:underline decoration-1 underline-offset-4">
                                    {article.title}
                                </h3>
                                <p class="text-xs text-gray-500 mb-4 leading-relaxed">
                                    {article.desc}
                                </p>
                                <a href="#" class="text-xs font-medium underline decoration-1 underline-offset-4">Read more</a>
                            </div>
                        {/each}
                    </div>
                </section>

            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-white pt-32 pb-12 border-t border-gray-100 relative overflow-hidden">
        <!-- Large Background Watermark -->
        <div class="absolute left-0 bottom-0 text-[20vw] font-bold text-gray-50 leading-none select-none pointer-events-none -mb-12 -ml-12">
            GS
        </div>

        <div class="max-w-[1600px] mx-auto px-6 relative z-10">
            <div class="flex flex-col md:flex-row justify-between items-end md:items-center mb-24">
                <div class="text-lg font-light text-gray-900">Transform your grant management</div>
                <div class="text-lg font-light underline decoration-1 underline-offset-4 text-gray-900">GRANTSCOPE.COM</div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-12 gap-8 items-end">
                <div class="md:col-span-6">
                    <!-- Logo -->
                    <div class="flex items-center gap-4 mb-4">
                        <div class="w-8 h-8 rounded-sm bg-primary-600 flex items-center justify-center">
                            <span class="text-white font-bold text-sm">GS</span>
                        </div>
                        <div class="text-xl font-semibold text-gray-900">
                            GrantScope
                        </div>
                    </div>
                    <p class="text-xs text-gray-500 max-w-sm">
                        AI-powered grant scoring and automated grantee reporting for foundations.
                    </p>
                </div>
                
                <div class="md:col-span-6 flex flex-col md:flex-row justify-between items-end md:items-end gap-8">
                    <div class="text-[10px] text-gray-400">
                        © 2025 GrantScope
                    </div>
                    
                    <div class="flex gap-8 text-[10px] font-medium uppercase tracking-wide text-gray-600">
                        <div class="flex flex-col gap-2">
                            <a href="#" class="hover:text-gray-900">About</a>
                            <a href="#" class="hover:text-gray-900">Product</a>
                            <a href="#" class="hover:text-gray-900">Contact</a>
                        </div>
                        <div class="flex flex-col gap-2">
                            <a href="#" class="hover:text-gray-900">Terms</a>
                            <a href="#" class="hover:text-gray-900">Privacy Policy</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</div>

<style>
    /* Custom scrollbar hide for clean look */
    ::-webkit-scrollbar {
        width: 0px;
        background: transparent;
    }
</style>

