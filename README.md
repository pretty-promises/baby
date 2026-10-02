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
