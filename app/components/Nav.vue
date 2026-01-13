<script setup></script>

<template>
  <nav
    class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 bg-white/95 backdrop-blur-md border-b border-slate-200 py-3">
    <div class="container mx-auto px-4 flex items-center justify-between">
      <a class="flex items-center gap-2 group" href="/">
        <span class="text-xl font-bold text-slate-900">NoPDF</span>
      </a>
      <div class="hidden md:flex items-center gap-8">
        <a
          class="text-sm font-semibold text-slate-600 hover:text-blue-600 transition-colors"
          href="/tools">
          All Tools
        </a>
        <a
          class="text-sm font-semibold text-slate-600 hover:text-blue-600 transition-colors"
          href="/tools/merge">
          Merge PDF
        </a>
        <a
          class="text-sm font-semibold text-slate-600 hover:text-blue-600 transition-colors"
          href="/tools/decrypt">
          Unlock PDF
        </a>
        <div class="flex items-center gap-3">
          <a
            class="px-5 py-2.5 bg-blue-600 text-white text-sm font-bold rounded-full hover:bg-blue-700 transition-all active:scale-95 shadow-lg shadow-blue-100"
            href="/tools">
            Get Started
          </a>
          <a
            href="https://github.com/hkn-33/NoPDF"
            target="_blank"
            rel="noopener noreferrer"
            class="p-2.5 bg-slate-900 text-white rounded-full hover:bg-slate-800 transition-all active:scale-95 shadow-lg shadow-slate-200 flex items-center justify-center"
            aria-label="GitHub Repository">
            Github
          </a>
          <a
            href="#"
            target="_blank"
            rel="noopener noreferrer"
            class="px-5 py-2.5 bg-[#FFDD00] text-slate-900 text-sm font-bold rounded-full hover:bg-[#FFCC00] transition-all active:scale-95 shadow-lg shadow-yellow-100 flex items-center gap-2">
            <span>☕</span>
            Buy me a coffee
          </a>
        </div>
      </div>
      <button
        class="md:hidden p-2 text-slate-600 hover:text-slate-900 transition-colors"
        aria-label="Toggle menu"></button>
    </div>
  </nav>
</template>
