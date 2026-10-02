Goal: Create a repository for our baby registry that has links to several sites they can buy from. 

Format: Follow Zola format or something like google shopping. Or like one of those blogs that has comparisons and shows you where to get everything. 

Image
Item Name
Item Button Link to Amazon
Item Button Link to Walmart
Item Button Link to Target

Create an inventory to track whether someone purchases the item. 
After someone clicks on a link, have a pop up ask them if they purchased the item and have a yes/no dialogue. If yes, then update the inventory to say sold. 

Navigation code 
 <!-- Navigation / Terminal Header -->
    <header class="sticky top-0 z-50 bg-expedition-navy text-white shadow-lg border-b-2 border-expedition-gold">
        <div class="max-w-6xl mx-auto px-4 py-3 flex flex-wrap items-center justify-between">
            <a href="#hero" class="flex items-center space-x-3 group">
                <div class="w-9 h-9 rounded-full bg-expedition-terracotta flex items-center justify-center text-white transform group-hover:rotate-45 transition-transform duration-300">
                    <i class="fa-solid fa-plane text-sm"></i>
                </div>
                <div>
                                

                    <span class="font-miltonian text-lg tracking-wide block leading-none">FLIGHT #BABY-2027</span>
                    <span class="font-mono text-xs text-expedition-gold tracking-widest uppercase">EXPEDITION PARENTHOOD</span>
                </div>
            </a>

            <!-- Terminal Style Nav Links -->
            <nav class="hidden md:flex items-center space-x-1 text-xs font-mono">
                <a href="#boarding-pass" class="px-3 py-1.5 rounded hover:bg-expedition-navylight transition-colors uppercase"><i class="fa-solid fa-ticket mr-1.5 text-expedition-gold"></i>Boarding Pass</a>
                <a href="#progress" class="px-3 py-1.5 rounded hover:bg-expedition-navylight transition-colors uppercase"><i class="fa-solid fa-route mr-1.5 text-expedition-gold"></i>Flight Tracker</a>
                <a href="#poll" class="px-3 py-1.5 rounded hover:bg-expedition-navylight transition-colors uppercase"><i class="fa-solid fa-vote-yea mr-1.5 text-expedition-gold"></i>Predictions</a>
                <a href="#gallery" class="px-3 py-1.5 rounded hover:bg-expedition-navylight transition-colors uppercase"><i class="fa-solid fa-camera-retro mr-1.5 text-expedition-gold"></i>Sightseeing Logs</a>
                <a href="#registry" class="px-3 py-1.5 rounded hover:bg-expedition-navylight transition-colors uppercase"><i class="fa-solid fa-suitcase mr-1.5 text-expedition-gold"></i>Gear Checklist</a>
                <a href="#guestbook" class="px-3 py-1.5 bg-expedition-terracotta hover:bg-opacity-90 text-white rounded transition-colors uppercase font-bold"><i class="fa-solid fa-passport mr-1.5"></i>Guestbook</a>
            </nav>

            <!-- Mobile menu trigger -->
            <button id="mobile-menu-btn" class="md:hidden text-expedition-sand focus:outline-none p-1">
                <i class="fa-solid fa-bars text-xl"></i>
            </button>
        </div>

        <!-- Mobile Navigation Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-expedition-navylight border-t border-slate-700 px-4 py-3 space-y-2 text-sm font-mono">
            <a href="#boarding-pass" class="mobile-link block py-2 border-b border-slate-700/50"><i class="fa-solid fa-ticket w-6 text-expedition-gold"></i> Boarding Pass</a>
            <a href="#progress" class="mobile-link block py-2 border-b border-slate-700/50"><i class="fa-solid fa-route w-6 text-expedition-gold"></i> Flight Tracker</a>
            <a href="#poll" class="mobile-link block py-2 border-b border-slate-700/50"><i class="fa-solid fa-vote-yea w-6 text-expedition-gold"></i> Departure Poll</a>
            <a href="#gallery" class="mobile-link block py-2 border-b border-slate-700/50"><i class="fa-solid fa-camera-retro w-6 text-expedition-gold"></i> Sightseeing Logs</a>
            <a href="#registry" class="mobile-link block py-2 border-b border-slate-700/50"><i class="fa-solid fa-suitcase w-6 text-expedition-gold"></i> Gear Checklist</a>
            <a href="#guestbook" class="mobile-link block py-2 text-expedition-gold font-bold"><i class="fa-solid fa-passport w-6"></i> Passport Guestbook</a>
        </div>
    </header>

     <!-- SECTION 6: PASSPORT STAMP GUESTBOOK -->
        <section id="guestbook" class="scroll-mt-20">
            <div class="bg-white rounded-2xl p-6 sm:p-8 shadow-md border border-expedition-parchment">
                <div class="text-center max-w-xl mx-auto mb-8">
                    <div class="w-12 h-12 rounded-full bg-expedition-sagelight text-expedition-sage flex items-center justify-center text-xl mx-auto mb-2">
                        <i class="fa-solid fa-passport"></i>
                    </div>
                    <h2 class="font-serif text-3xl font-bold text-expedition-navy">Passport Guestbook</h2>
                    <p class="text-slate-600 text-sm mt-1">Leave a message or advice for our journey! Each note receives an official stamped passport entry.</p>
                </div>

                <!-- Form & Recent Messages Container -->
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
                    
                    <!-- Form Column -->
                    <form id="guestbook-form" class="lg:col-span-5 bg-expedition-sand p-6 rounded-xl border border-expedition-kraft space-y-4">
                        <h3 class="font-serif font-bold text-lg text-expedition-navy flex items-center">
                            <i class="fa-solid fa-pen-nib mr-2 text-expedition-terracotta"></i> Stamp Your Entry
                        </h3>

                        <div>
                            <label for="gb-name" class="block font-mono text-xs text-slate-600 mb-1">TRAVELER / YOUR NAME *</label>
                            <input type="text" id="gb-name" required placeholder="Aunt Sarah & Uncle Dave" class="w-full px-3 py-2 rounded-lg border border-slate-300 focus:outline-none focus:ring-2 focus:ring-expedition-terracotta text-sm">
                        </div>

                        <div>
                            <label for="gb-location" class="block font-mono text-xs text-slate-600 mb-1">DEPARTING FROM (LOCATION)</label>
                            <input type="text" id="gb-location" placeholder="Chicago, IL" class="w-full px-3 py-2 rounded-lg border border-slate-300 focus:outline-none focus:ring-2 focus:ring-expedition-terracotta text-sm">
                        </div>

                        <div>
                            <label for="gb-message" class="block font-mono text-xs text-slate-600 mb-1">WELL WISHES / ADVICE *</label>
                            <textarea id="gb-message" required rows="3" placeholder="Bon voyage into parenthood! Stock up on coffee..." class="w-full px-3 py-2 rounded-lg border border-slate-300 focus:outline-none focus:ring-2 focus:ring-expedition-terracotta text-sm"></textarea>
                        </div>

                        <button type="submit" class="w-full py-3 bg-expedition-navy hover:bg-expedition-navylight text-white font-mono text-xs font-bold uppercase rounded-lg transition-colors shadow-md flex items-center justify-center space-x-2">
                            <i class="fa-solid fa-stamp text-expedition-gold"></i>
                            <span>Stamp Passport</span>
                        </button>
                    </form>

                    <!-- Stamp Notes Feed Column -->
                    <div class="lg:col-span-7 space-y-4">
                        <h3 class="font-mono text-xs text-slate-400 uppercase tracking-widest font-bold">RECENT PASSPORT STAMPS</h3>
                        
                        <div id="guestbook-list" class="space-y-4 max-h-[480px] overflow-y-auto pr-2">
                        </div>
                    </div>

                </div>
            </div>
        </section>
