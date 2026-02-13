<!doctype html>
<html lang="en" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CoolShift - AI Climate Scheduler</title>
  <script src="https://cdn.tailwindcss.com/3.4.17"></script>
  <script src="/_sdk/data_sdk.js"></script>
  <script src="/_sdk/element_sdk.js"></script>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&amp;family=JetBrains+Mono:wght@400;500&amp;display=swap" rel="stylesheet">
  <style>
    * { font-family: 'Space Grotesk', sans-serif; }
    .mono { font-family: 'JetBrains Mono', monospace; }
    
    @keyframes pulse-glow {
      0%, 100% { box-shadow: 0 0 20px rgba(34, 197, 94, 0.3); }
      50% { box-shadow: 0 0 40px rgba(34, 197, 94, 0.6); }
    }
    
    @keyframes water-flow {
      0% { transform: translateY(100%); opacity: 0; }
      50% { opacity: 1; }
      100% { transform: translateY(-100%); opacity: 0; }
    }
    
    @keyframes float {
      0%, 100% { transform: translateY(0px); }
      50% { transform: translateY(-10px); }
    }
    
    @keyframes shimmer {
      0% { background-position: -200% 0; }
      100% { background-position: 200% 0; }
    }
    
    .animate-pulse-glow { animation: pulse-glow 2s ease-in-out infinite; }
    .animate-water { animation: water-flow 3s ease-in-out infinite; }
    .animate-float { animation: float 3s ease-in-out infinite; }
    
    .shimmer-bg {
      background: linear-gradient(90deg, transparent 0%, rgba(255,255,255,0.1) 50%, transparent 100%);
      background-size: 200% 100%;
      animation: shimmer 2s infinite;
    }
    
    .water-meter-fill {
      transition: height 1s ease-out;
    }
    
    .card-hover {
      transition: all 0.3s ease;
    }
    .card-hover:hover {
      transform: translateY(-4px);
    }
    
    .gradient-text {
      background: linear-gradient(135deg, #22c55e 0%, #06b6d4 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }
    
    .glass {
      background: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    input, select {
      transition: all 0.2s ease;
    }
    input:focus, select:focus {
      outline: none;
      border-color: #22c55e;
      box-shadow: 0 0 0 3px rgba(34, 197, 94, 0.2);
    }
    
    .btn-primary {
      background: linear-gradient(135deg, #22c55e 0%, #16a34a 100%);
      transition: all 0.3s ease;
    }
    .btn-primary:hover {
      transform: scale(1.02);
      box-shadow: 0 10px 30px rgba(34, 197, 94, 0.4);
    }
    
    .progress-ring {
      transform: rotate(-90deg);
    }
    
    ::-webkit-scrollbar { width: 8px; }
    ::-webkit-scrollbar-track { background: rgba(255,255,255,0.05); border-radius: 4px; }
    ::-webkit-scrollbar-thumb { background: rgba(34, 197, 94, 0.5); border-radius: 4px; }
    ::-webkit-scrollbar-thumb:hover { background: rgba(34, 197, 94, 0.7); }
  </style>
  <style>body { box-sizing: border-box; }</style>
 </head>
 <body class="h-full bg-slate-950 text-white">
  <div id="app" class="h-full w-full overflow-auto"><!-- Animated Background -->
   <div class="fixed inset-0 overflow-hidden pointer-events-none">
    <div class="absolute top-0 left-1/4 w-96 h-96 bg-green-500/10 rounded-full blur-3xl"></div>
    <div class="absolute bottom-0 right-1/4 w-96 h-96 bg-cyan-500/10 rounded-full blur-3xl"></div>
    <div class="absolute top-1/2 left-1/2 w-64 h-64 bg-emerald-500/5 rounded-full blur-2xl animate-float"></div>
   </div>
   <div class="relative z-10 min-h-full p-4 md:p-6 lg:p-8"><!-- Header -->
    <header class="mb-8">
     <div class="flex flex-col md:flex-row md:items-center md:justify-between gap-4">
      <div class="flex items-center gap-4">
       <div class="relative">
        <div class="w-14 h-14 rounded-2xl bg-gradient-to-br from-green-500 to-cyan-500 flex items-center justify-center animate-pulse-glow">
         <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20 7l-8-4-8 4m16 0l-8 4m8-4v10l-8 4m0-10L4 7m8 4v10M4 7v10l8 4" />
         </svg>
        </div>
        <div class="absolute -top-1 -right-1 w-4 h-4 bg-green-400 rounded-full border-2 border-slate-950"></div>
       </div>
       <div>
        <h1 id="app-title" class="text-2xl md:text-3xl font-bold gradient-text">CoolShift</h1>
        <p id="app-tagline" class="text-slate-400 text-sm">AI-Powered Climate-Aware Scheduling</p>
       </div>
      </div><!-- User Stats Badge -->
      <div class="glass rounded-2xl px-6 py-3 flex items-center gap-6">
       <div class="flex items-center gap-2">
        <div class="w-8 h-8 rounded-full bg-gradient-to-br from-yellow-400 to-orange-500 flex items-center justify-center"><span class="text-sm">🏆</span>
        </div>
        <div>
         <p class="text-xs text-slate-400">Level</p>
         <p id="user-level" class="text-sm font-semibold text-yellow-400">Beginner</p>
        </div>
       </div>
       <div class="h-8 w-px bg-slate-700"></div>
       <div class="flex items-center gap-2"><span class="text-xl">🌱</span>
        <div>
         <p class="text-xs text-slate-400">Green Credits</p>
         <p id="total-credits" class="text-sm font-semibold text-green-400 mono">0</p>
        </div>
       </div>
      </div>
     </div>
    </header><!-- Main Grid -->
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-6"><!-- Left Column: Scheduler -->
     <div class="lg:col-span-2 space-y-6"><!-- Workload Scheduler Card -->
      <div class="glass rounded-3xl p-6 card-hover">
       <div class="flex items-center gap-3 mb-6">
        <div class="w-10 h-10 rounded-xl bg-green-500/20 flex items-center justify-center">
         <svg class="w-5 h-5 text-green-400" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2" />
         </svg>
        </div>
        <div>
         <h2 class="text-xl font-semibold">Schedule New Workload</h2>
         <p class="text-slate-400 text-sm">AI will optimize for minimum water consumption</p>
        </div>
       </div>
       <form id="workload-form" class="space-y-4">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
         <div><label for="workload-name" class="block text-sm font-medium text-slate-300 mb-2">Workload Name</label> <input type="text" id="workload-name" placeholder="e.g., ML Training Job" class="w-full px-4 py-3 bg-slate-800/50 border border-slate-700 rounded-xl text-white placeholder-slate-500">
         </div>
         <div><label for="workload-intensity" class="block text-sm font-medium text-slate-300 mb-2">Intensity</label> <select id="workload-intensity" class="w-full px-4 py-3 bg-slate-800/50 border border-slate-700 rounded-xl text-white"> <option value="light">Light (Web Hosting)</option> <option value="medium">Medium (Data Processing)</option> <option value="heavy" selected>Heavy (AI/ML Training)</option> </select>
         </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
         <div><label for="original-location" class="block text-sm font-medium text-slate-300 mb-2">📍 Preferred Location</label> <select id="original-location" class="w-full px-4 py-3 bg-slate-800/50 border border-slate-700 rounded-xl text-white"> <option value="delhi">Delhi (High Water Stress)</option> <option value="mumbai">Mumbai (Moderate)</option> <option value="bangalore">Bangalore (Moderate)</option> <option value="hyderabad">Hyderabad (Low)</option> <option value="chennai">Chennai (Moderate)</option> </select>
         </div>
         <div><label for="original-time" class="block text-sm font-medium text-slate-300 mb-2">🕒 Preferred Time</label> <select id="original-time" class="w-full px-4 py-3 bg-slate-800/50 border border-slate-700 rounded-xl text-white"> <option value="morning">Morning (6 AM - 12 PM)</option> <option value="afternoon" selected>Afternoon (12 PM - 6 PM)</option> <option value="evening">Evening (6 PM - 10 PM)</option> <option value="night">Night (10 PM - 6 AM)</option> </select>
         </div>
        </div>
        <div><label for="cooling-type" class="block text-sm font-medium text-slate-300 mb-2">❄️ Cooling Method</label> <select id="cooling-type" class="w-full px-4 py-3 bg-slate-800/50 border border-slate-700 rounded-xl text-white"> <option value="evaporative">Evaporative Cooling (High Water)</option> <option value="chilled">Chilled Water System (Medium)</option> <option value="air">Air Cooling (Low Water)</option> <option value="hybrid">Hybrid System (Variable)</option> </select>
        </div><button type="submit" id="submit-btn" class="w-full btn-primary py-4 rounded-xl font-semibold text-white flex items-center justify-center gap-2">
         <svg class="w-5 h-5" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
         </svg><span>Optimize &amp; Schedule</span> </button>
       </form>
      </div><!-- AI Prediction Result -->
      <div id="prediction-result" class="hidden glass rounded-3xl p-6 border-2 border-green-500/30 card-hover">
       <div class="flex items-center gap-3 mb-6">
        <div class="w-10 h-10 rounded-xl bg-cyan-500/20 flex items-center justify-center animate-float"><span class="text-xl">🧠</span>
        </div>
        <div>
         <h3 class="text-lg font-semibold">AI Optimization Result</h3>
         <p class="text-slate-400 text-sm">Predictive analysis complete</p>
        </div>
       </div>
       <div class="grid grid-cols-1 md:grid-cols-2 gap-6"><!-- Original Plan -->
        <div class="bg-red-500/10 border border-red-500/30 rounded-2xl p-4">
         <div class="flex items-center gap-2 mb-3"><span class="text-red-400">⚠️</span> <span class="text-red-400 font-medium">Original Plan</span>
         </div>
         <div class="space-y-2 text-sm">
          <p><span class="text-slate-400">Location:</span> <span id="orig-loc" class="text-white font-medium">Delhi</span></p>
          <p><span class="text-slate-400">Time:</span> <span id="orig-time" class="text-white font-medium">2 PM</span></p>
          <p><span class="text-slate-400">Water Use:</span> <span id="orig-water" class="text-red-400 font-bold mono">14,200 L</span></p>
         </div>
        </div><!-- Optimized Plan -->
        <div class="bg-green-500/10 border border-green-500/30 rounded-2xl p-4">
         <div class="flex items-center gap-2 mb-3"><span class="text-green-400">✔️</span> <span class="text-green-400 font-medium">AI Optimized</span>
         </div>
         <div class="space-y-2 text-sm">
          <p><span class="text-slate-400">Location:</span> <span id="opt-loc" class="text-white font-medium">Hyderabad</span></p>
          <p><span class="text-slate-400">Time:</span> <span id="opt-time" class="text-white font-medium">9 PM</span></p>
          <p><span class="text-slate-400">Water Use:</span> <span id="opt-water" class="text-green-400 font-bold mono">7,800 L</span></p>
         </div>
        </div>
       </div><!-- Savings Display -->
       <div class="mt-6 bg-gradient-to-r from-green-500/20 to-cyan-500/20 rounded-2xl p-4 text-center">
        <p class="text-slate-300 mb-1">Total Water Savings</p>
        <p class="text-4xl font-bold gradient-text mono" id="savings-display">45%</p>
        <p class="text-sm text-slate-400 mt-2">💧 <span id="liters-saved">6,400</span> Litres saved • <span id="credits-earned">64</span> Green Credits earned</p>
       </div><button id="accept-optimization" class="w-full mt-4 btn-primary py-3 rounded-xl font-semibold text-white"> Accept Optimization &amp; Schedule </button>
      </div><!-- Scheduled Workloads -->
      <div class="glass rounded-3xl p-6">
       <div class="flex items-center justify-between mb-6">
        <div class="flex items-center gap-3">
         <div class="w-10 h-10 rounded-xl bg-purple-500/20 flex items-center justify-center">
          <svg class="w-5 h-5 text-purple-400" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
          </svg>
         </div>
         <div>
          <h3 class="text-lg font-semibold">Scheduled Workloads</h3>
          <p class="text-slate-400 text-sm" id="workload-count">0 active workloads</p>
         </div>
        </div>
       </div>
       <div id="workloads-list" class="space-y-3 max-h-80 overflow-y-auto">
        <div class="text-center py-8 text-slate-500"><span class="text-4xl mb-2 block">📋</span>
         <p>No workloads scheduled yet</p>
         <p class="text-sm">Schedule your first workload above</p>
        </div>
       </div>
      </div>
     </div><!-- Right Column: Stats & Gamification -->
     <div class="space-y-6"><!-- Water Meter -->
      <div class="glass rounded-3xl p-6 card-hover">
       <div class="flex items-center gap-3 mb-6">
        <div class="w-10 h-10 rounded-xl bg-cyan-500/20 flex items-center justify-center"><span class="text-xl">💧</span>
        </div>
        <div>
         <h3 class="text-lg font-semibold">Water Impact Meter</h3>
         <p class="text-slate-400 text-sm">Total savings this month</p>
        </div>
       </div>
       <div class="relative flex justify-center mb-4">
        <div class="relative w-40 h-56 bg-slate-800/50 rounded-3xl border-2 border-cyan-500/30 overflow-hidden">
         <div id="water-meter-fill" class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-cyan-500 to-cyan-300 water-meter-fill" style="height: 0%">
          <div class="absolute inset-0 shimmer-bg"></div>
         </div>
         <div class="absolute inset-0 flex items-center justify-center">
          <div class="text-center">
           <p id="total-water-saved" class="text-3xl font-bold text-white mono">0</p>
           <p class="text-sm text-slate-300">Litres Saved</p>
          </div>
         </div><!-- Water Bubbles -->
         <div class="absolute bottom-4 left-4 w-3 h-3 bg-white/30 rounded-full animate-water" style="animation-delay: 0s;"></div>
         <div class="absolute bottom-4 right-6 w-2 h-2 bg-white/30 rounded-full animate-water" style="animation-delay: 0.5s;"></div>
         <div class="absolute bottom-4 left-1/2 w-2 h-2 bg-white/30 rounded-full animate-water" style="animation-delay: 1s;"></div>
        </div>
       </div>
       <div class="text-center">
        <p class="text-sm text-slate-400">Equivalent to supporting</p>
        <p class="text-xl font-semibold text-cyan-400"><span id="households-supported">0</span> households for a day</p>
       </div>
      </div><!-- Green Credits Progress -->
      <div class="glass rounded-3xl p-6 card-hover">
       <div class="flex items-center gap-3 mb-6">
        <div class="w-10 h-10 rounded-xl bg-yellow-500/20 flex items-center justify-center"><span class="text-xl">🏅</span>
        </div>
        <div>
         <h3 class="text-lg font-semibold">Level Progress</h3>
         <p class="text-slate-400 text-sm">Earn credits to level up</p>
        </div>
       </div>
       <div class="flex justify-center mb-4">
        <div class="relative">
         <svg class="w-32 h-32 progress-ring"><circle cx="64" cy="64" r="56" stroke="#1e293b" stroke-width="8" fill="none" /> <circle id="progress-circle" cx="64" cy="64" r="56" stroke="url(#progressGradient)" stroke-width="8" fill="none" stroke-dasharray="351.86" stroke-dashoffset="351.86" stroke-linecap="round" /> <defs>
           <lineargradient id="progressGradient" x1="0%" y1="0%" x2="100%" y2="0%">
            <stop offset="0%" stop-color="#22c55e" />
            <stop offset="100%" stop-color="#06b6d4" />
           </lineargradient>
          </defs>
         </svg>
         <div class="absolute inset-0 flex items-center justify-center">
          <div class="text-center">
           <p id="level-credits" class="text-2xl font-bold mono text-white">0</p>
           <p class="text-xs text-slate-400">/ 100</p>
          </div>
         </div>
        </div>
       </div>
       <div class="space-y-3">
        <div class="flex items-center justify-between text-sm"><span class="text-slate-400">Current Level</span> <span id="current-level-badge" class="px-3 py-1 bg-slate-700 rounded-full text-slate-300">Beginner</span>
        </div>
        <div class="flex items-center justify-between text-sm"><span class="text-slate-400">Next Level</span> <span id="next-level-badge" class="px-3 py-1 bg-green-500/20 rounded-full text-green-400">Water Saver</span>
        </div>
       </div>
      </div><!-- Achievements -->
      <div class="glass rounded-3xl p-6 card-hover">
       <div class="flex items-center gap-3 mb-6">
        <div class="w-10 h-10 rounded-xl bg-orange-500/20 flex items-center justify-center"><span class="text-xl">🎖️</span>
        </div>
        <div>
         <h3 class="text-lg font-semibold">Achievements</h3>
         <p class="text-slate-400 text-sm">Badges earned</p>
        </div>
       </div>
       <div id="badges-container" class="grid grid-cols-3 gap-3">
        <div class="aspect-square rounded-xl bg-slate-800/50 border border-slate-700 flex items-center justify-center opacity-30" title="First Schedule"><span class="text-2xl">🌱</span>
        </div>
        <div class="aspect-square rounded-xl bg-slate-800/50 border border-slate-700 flex items-center justify-center opacity-30" title="10 Workloads"><span class="text-2xl">💧</span>
        </div>
        <div class="aspect-square rounded-xl bg-slate-800/50 border border-slate-700 flex items-center justify-center opacity-30" title="1000L Saved"><span class="text-2xl">🌊</span>
        </div>
        <div class="aspect-square rounded-xl bg-slate-800/50 border border-slate-700 flex items-center justify-center opacity-30" title="Night Owl"><span class="text-2xl">🦉</span>
        </div>
        <div class="aspect-square rounded-xl bg-slate-800/50 border border-slate-700 flex items-center justify-center opacity-30" title="Multi-Region"><span class="text-2xl">🗺️</span>
        </div>
        <div class="aspect-square rounded-xl bg-slate-800/50 border border-slate-700 flex items-center justify-center opacity-30" title="Champion"><span class="text-2xl">🏆</span>
        </div>
       </div>
      </div><!-- Regional Water Stress -->
      <div class="glass rounded-3xl p-6 card-hover">
       <div class="flex items-center gap-3 mb-4">
        <div class="w-10 h-10 rounded-xl bg-red-500/20 flex items-center justify-center"><span class="text-xl">🗺️</span>
        </div>
        <div>
         <h3 class="text-lg font-semibold">Regional Water Stress</h3>
         <p class="text-slate-400 text-sm">India data centers</p>
        </div>
       </div>
       <div class="space-y-2">
        <div class="flex items-center justify-between p-2 rounded-lg bg-red-500/10"><span class="text-sm">Delhi</span>
         <div class="flex items-center gap-2">
          <div class="w-16 h-2 bg-slate-700 rounded-full overflow-hidden">
           <div class="h-full bg-red-500 rounded-full" style="width: 90%"></div>
          </div><span class="text-xs text-red-400">High</span>
         </div>
        </div>
        <div class="flex items-center justify-between p-2 rounded-lg bg-yellow-500/10"><span class="text-sm">Mumbai</span>
         <div class="flex items-center gap-2">
          <div class="w-16 h-2 bg-slate-700 rounded-full overflow-hidden">
           <div class="h-full bg-yellow-500 rounded-full" style="width: 60%"></div>
          </div><span class="text-xs text-yellow-400">Moderate</span>
         </div>
        </div>
        <div class="flex items-center justify-between p-2 rounded-lg bg-yellow-500/10"><span class="text-sm">Bangalore</span>
         <div class="flex items-center gap-2">
          <div class="w-16 h-2 bg-slate-700 rounded-full overflow-hidden">
           <div class="h-full bg-yellow-500 rounded-full" style="width: 55%"></div>
          </div><span class="text-xs text-yellow-400">Moderate</span>
         </div>
        </div>
        <div class="flex items-center justify-between p-2 rounded-lg bg-green-500/10"><span class="text-sm">Hyderabad</span>
         <div class="flex items-center gap-2">
          <div class="w-16 h-2 bg-slate-700 rounded-full overflow-hidden">
           <div class="h-full bg-green-500 rounded-full" style="width: 35%"></div>
          </div><span class="text-xs text-green-400">Low</span>
         </div>
        </div>
        <div class="flex items-center justify-between p-2 rounded-lg bg-yellow-500/10"><span class="text-sm">Chennai</span>
         <div class="flex items-center gap-2">
          <div class="w-16 h-2 bg-slate-700 rounded-full overflow-hidden">
           <div class="h-full bg-yellow-500 rounded-full" style="width: 50%"></div>
          </div><span class="text-xs text-yellow-400">Moderate</span>
         </div>
        </div>
       </div>
      </div>
     </div>
    </div><!-- Footer -->
    <footer class="mt-8 text-center text-slate-500 text-sm">
     <p>🌊 CoolShift — Predicting water impact before execution begins</p>
    </footer>
   </div>
  </div><!-- Loading Overlay -->
  <div id="loading-overlay" class="hidden fixed inset-0 bg-slate-950/80 z-50 flex items-center justify-center">
   <div class="text-center">
    <div class="w-16 h-16 border-4 border-green-500 border-t-transparent rounded-full animate-spin mx-auto mb-4"></div>
    <p class="text-white font-medium">Processing...</p>
   </div>
  </div>
  <script>
    // Configuration and constants
    const defaultConfig = {
      app_title: 'CoolShift',
      tagline: 'AI-Powered Climate-Aware Scheduling',
      background_color: '#020617',
      surface_color: '#0f172a',
      text_color: '#f8fafc',
      primary_action_color: '#22c55e',
      secondary_action_color: '#06b6d4'
    };

    let config = { ...defaultConfig };
    let workloads = [];
    let pendingOptimization = null;
    let currentRecordCount = 0;

    // Regional data for AI optimization
    const regionData = {
      delhi: { name: 'Delhi', waterStress: 0.9, baseTemp: 38, coolingEfficiency: 0.6 },
      mumbai: { name: 'Mumbai', waterStress: 0.6, baseTemp: 32, coolingEfficiency: 0.75 },
      bangalore: { name: 'Bangalore', waterStress: 0.55, baseTemp: 28, coolingEfficiency: 0.85 },
      hyderabad: { name: 'Hyderabad', waterStress: 0.35, baseTemp: 30, coolingEfficiency: 0.9 },
      chennai: { name: 'Chennai', waterStress: 0.5, baseTemp: 33, coolingEfficiency: 0.8 }
    };

    const timeSlots = {
      morning: { name: 'Morning (6 AM - 12 PM)', tempMultiplier: 0.85, label: '9 AM' },
      afternoon: { name: 'Afternoon (12 PM - 6 PM)', tempMultiplier: 1.2, label: '2 PM' },
      evening: { name: 'Evening (6 PM - 10 PM)', tempMultiplier: 0.9, label: '7 PM' },
      night: { name: 'Night (10 PM - 6 AM)', tempMultiplier: 0.7, label: '11 PM' }
    };

    const intensityMultipliers = { light: 0.4, medium: 0.7, heavy: 1.0 };
    const coolingMultipliers = { evaporative: 1.3, chilled: 1.0, air: 0.5, hybrid: 0.8 };

    const levels = [
      { name: 'Beginner', minCredits: 0, color: 'slate' },
      { name: 'Water Saver', minCredits: 100, color: 'green' },
      { name: 'Eco Optimizer', minCredits: 500, color: 'cyan' },
      { name: 'Sustainability Champion', minCredits: 1000, color: 'yellow' }
    ];

    // Calculate water usage
    function calculateWaterUsage(location, time, intensity, cooling) {
      const region = regionData[location];
      const timeSlot = timeSlots[time];
      const baseWater = 10000;
      
      const waterUsage = baseWater 
        * region.waterStress 
        * (1 / region.coolingEfficiency)
        * timeSlot.tempMultiplier 
        * intensityMultipliers[intensity]
        * coolingMultipliers[cooling];
      
      return Math.round(waterUsage);
    }

    // AI Optimization - find best location and time
    function findOptimalSchedule(intensity, cooling, excludeLocation, excludeTime) {
      let bestOption = { location: null, time: null, waterUsage: Infinity };
      
      for (const loc of Object.keys(regionData)) {
        for (const time of Object.keys(timeSlots)) {
          const usage = calculateWaterUsage(loc, time, intensity, cooling);
          if (usage < bestOption.waterUsage) {
            bestOption = { location: loc, time: time, waterUsage: usage };
          }
        }
      }
      
      return bestOption;
    }

    // Calculate green credits from water saved
    function calculateGreenCredits(waterSaved) {
      return Math.round(waterSaved / 100);
    }

    // Get user level based on total credits
    function getUserLevel(totalCredits) {
      let currentLevel = levels[0];
      let nextLevel = levels[1];
      
      for (let i = levels.length - 1; i >= 0; i--) {
        if (totalCredits >= levels[i].minCredits) {
          currentLevel = levels[i];
          nextLevel = levels[i + 1] || null;
          break;
        }
      }
      
      return { current: currentLevel, next: nextLevel };
    }

    // Data Handler for SDK
    const dataHandler = {
      onDataChanged(data) {
        workloads = data;
        currentRecordCount = data.length;
        renderWorkloads();
        updateStats();
        updateBadges();
      }
    };

    // Render workloads list
    function renderWorkloads() {
      const container = document.getElementById('workloads-list');
      const countEl = document.getElementById('workload-count');
      
      countEl.textContent = `${workloads.length} active workload${workloads.length !== 1 ? 's' : ''}`;
      
      if (workloads.length === 0) {
        container.innerHTML = `
          <div class="text-center py-8 text-slate-500">
            <span class="text-4xl mb-2 block">📋</span>
            <p>No workloads scheduled yet</p>
            <p class="text-sm">Schedule your first workload above</p>
          </div>
        `;
        return;
      }
      
      container.innerHTML = workloads.map(w => `
        <div class="bg-slate-800/50 rounded-xl p-4 border border-slate-700" data-id="${w.__backendId}">
          <div class="flex items-start justify-between">
            <div class="flex-1">
              <div class="flex items-center gap-2 mb-2">
                <span class="text-green-400">✔️</span>
                <span class="font-medium">${escapeHtml(w.workload_name)}</span>
                <span class="px-2 py-0.5 text-xs rounded-full ${w.status === 'optimized' ? 'bg-green-500/20 text-green-400' : 'bg-slate-600 text-slate-300'}">${w.status}</span>
              </div>
              <div class="grid grid-cols-2 gap-x-4 gap-y-1 text-sm">
                <p class="text-slate-400">📍 ${escapeHtml(w.optimized_location)}</p>
                <p class="text-slate-400">🕒 ${escapeHtml(w.optimized_time)}</p>
                <p class="text-green-400">💧 ${w.optimized_water.toLocaleString()}L</p>
                <p class="text-cyan-400">🌱 +${w.green_credits} credits</p>
              </div>
              <p class="text-xs text-slate-500 mt-2">Saved ${w.savings_percent}% (${w.water_saved.toLocaleString()}L) vs original plan</p>
            </div>
            <button onclick="deleteWorkload('${w.__backendId}')" class="text-slate-500 hover:text-red-400 transition-colors p-1" title="Delete">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 7l-.867 12.142A2 2 0 0116.138 21H7.862a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16"/>
              </svg>
            </button>
          </div>
        </div>
      `).join('');
    }

    // Update stats displays
    function updateStats() {
      const totalWaterSaved = workloads.reduce((sum, w) => sum + w.water_saved, 0);
      const totalCredits = workloads.reduce((sum, w) => sum + w.green_credits, 0);
      const { current, next } = getUserLevel(totalCredits);
      
      // Water meter
      const maxWater = 50000;
      const meterPercent = Math.min((totalWaterSaved / maxWater) * 100, 100);
      document.getElementById('water-meter-fill').style.height = `${meterPercent}%`;
      document.getElementById('total-water-saved').textContent = totalWaterSaved.toLocaleString();
      document.getElementById('households-supported').textContent = Math.round(totalWaterSaved / 200);
      
      // Credits and levels
      document.getElementById('total-credits').textContent = totalCredits.toLocaleString();
      document.getElementById('user-level').textContent = current.name;
      document.getElementById('current-level-badge').textContent = current.name;
      document.getElementById('next-level-badge').textContent = next ? next.name : 'Max Level';
      
      // Progress ring
      const progressToNext = next ? (totalCredits - current.minCredits) / (next.minCredits - current.minCredits) : 1;
      const dashOffset = 351.86 * (1 - progressToNext);
      document.getElementById('progress-circle').style.strokeDashoffset = dashOffset;
      document.getElementById('level-credits').textContent = next ? (totalCredits - current.minCredits) : totalCredits;
    }

    // Update badges
    function updateBadges() {
      const container = document.getElementById('badges-container');
      const badges = container.querySelectorAll('div');
      const totalWaterSaved = workloads.reduce((sum, w) => sum + w.water_saved, 0);
      const totalCredits = workloads.reduce((sum, w) => sum + w.green_credits, 0);
      const hasNightSchedule = workloads.some(w => w.optimized_time.includes('11 PM') || w.optimized_time.includes('Night'));
      const uniqueRegions = new Set(workloads.map(w => w.optimized_location)).size;
      
      // First Schedule badge
      if (workloads.length >= 1) badges[0].classList.remove('opacity-30');
      // 10 Workloads badge
      if (workloads.length >= 10) badges[1].classList.remove('opacity-30');
      // 1000L Saved badge
      if (totalWaterSaved >= 1000) badges[2].classList.remove('opacity-30');
      // Night Owl badge
      if (hasNightSchedule) badges[3].classList.remove('opacity-30');
      // Multi-Region badge
      if (uniqueRegions >= 3) badges[4].classList.remove('opacity-30');
      // Champion badge
      if (totalCredits >= 1000) badges[5].classList.remove('opacity-30');
    }

    // Show loading overlay
    function showLoading(show) {
      document.getElementById('loading-overlay').classList.toggle('hidden', !show);
    }

    // Delete workload
    async function deleteWorkload(id) {
      const workload = workloads.find(w => w.__backendId === id);
      if (!workload) return;
      
      // Simple inline confirmation
      const btn = document.querySelector(`[data-id="${id}"] button`);
      if (btn.dataset.confirming !== 'true') {
        btn.dataset.confirming = 'true';
        btn.innerHTML = '<span class="text-red-400 text-xs">Click again to delete</span>';
        setTimeout(() => {
          if (btn) {
            btn.dataset.confirming = 'false';
            btn.innerHTML = `<svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 7l-.867 12.142A2 2 0 0116.138 21H7.862a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16"/>
            </svg>`;
          }
        }, 3000);
        return;
      }
      
      showLoading(true);
      const result = await window.dataSdk.delete(workload);
      showLoading(false);
      
      if (!result.isOk) {
        showToast('Failed to delete workload', 'error');
      }
    }

    // Show toast message
    function showToast(message, type = 'success') {
      const toast = document.createElement('div');
      toast.className = `fixed bottom-4 right-4 px-6 py-3 rounded-xl z-50 ${type === 'error' ? 'bg-red-500' : 'bg-green-500'} text-white font-medium shadow-lg`;
      toast.textContent = message;
      document.body.appendChild(toast);
      setTimeout(() => toast.remove(), 3000);
    }

    // Escape HTML
    function escapeHtml(str) {
      if (!str) return '';
      return str.replace(/[&<>"']/g, m => ({
        '&': '&amp;', '<': '&lt;', '>': '&gt;', '"': '&quot;', "'": '&#39;'
      }[m]));
    }

    // Form submission handler
    async function handleFormSubmit(e) {
      e.preventDefault();
      
      if (currentRecordCount >= 999) {
        showToast('Maximum limit of 999 workloads reached. Please delete some first.', 'error');
        return;
      }
      
      const name = document.getElementById('workload-name').value.trim();
      const intensity = document.getElementById('workload-intensity').value;
      const location = document.getElementById('original-location').value;
      const time = document.getElementById('original-time').value;
      const cooling = document.getElementById('cooling-type').value;
      
      if (!name) {
        showToast('Please enter a workload name', 'error');
        return;
      }
      
      // Calculate original water usage
      const originalWater = calculateWaterUsage(location, time, intensity, cooling);
      
      // Find optimal schedule
      const optimal = findOptimalSchedule(intensity, cooling, location, time);
      
      // Calculate savings
      const waterSaved = originalWater - optimal.waterUsage;
      const savingsPercent = Math.round((waterSaved / originalWater) * 100);
      const greenCredits = calculateGreenCredits(waterSaved);
      
      // Store pending optimization
      pendingOptimization = {
        workload_name: name,
        original_location: regionData[location].name,
        original_time: timeSlots[time].label,
        optimized_location: regionData[optimal.location].name,
        optimized_time: timeSlots[optimal.time].label,
        original_water: originalWater,
        optimized_water: optimal.waterUsage,
        water_saved: waterSaved,
        savings_percent: savingsPercent,
        green_credits: greenCredits,
        status: 'optimized'
      };
      
      // Show prediction result
      document.getElementById('orig-loc').textContent = regionData[location].name;
      document.getElementById('orig-time').textContent = timeSlots[time].label;
      document.getElementById('orig-water').textContent = originalWater.toLocaleString() + ' L';
      document.getElementById('opt-loc').textContent = regionData[optimal.location].name;
      document.getElementById('opt-time').textContent = timeSlots[optimal.time].label;
      document.getElementById('opt-water').textContent = optimal.waterUsage.toLocaleString() + ' L';
      document.getElementById('savings-display').textContent = savingsPercent + '%';
      document.getElementById('liters-saved').textContent = waterSaved.toLocaleString();
      document.getElementById('credits-earned').textContent = greenCredits;
      
      document.getElementById('prediction-result').classList.remove('hidden');
      document.getElementById('prediction-result').scrollIntoView({ behavior: 'smooth' });
    }

    // Accept optimization
    async function acceptOptimization() {
      if (!pendingOptimization) return;
      
      showLoading(true);
      
      const record = {
        ...pendingOptimization,
        id: Date.now().toString(),
        created_at: new Date().toISOString()
      };
      
      const result = await window.dataSdk.create(record);
      showLoading(false);
      
      if (result.isOk) {
        showToast('Workload scheduled successfully! 🎉');
        document.getElementById('prediction-result').classList.add('hidden');
        document.getElementById('workload-form').reset();
        pendingOptimization = null;
      } else {
        showToast('Failed to schedule workload', 'error');
      }
    }

    // Apply config to UI
    function applyConfig() {
      document.getElementById('app-title').textContent = config.app_title || defaultConfig.app_title;
      document.getElementById('app-tagline').textContent = config.tagline || defaultConfig.tagline;
    }

    // Element SDK initialization
    async function initElementSdk() {
      if (window.elementSdk) {
        window.elementSdk.init({
          defaultConfig,
          onConfigChange: async (newConfig) => {
            config = { ...defaultConfig, ...newConfig };
            applyConfig();
          },
          mapToCapabilities: (cfg) => ({
            recolorables: [
              {
                get: () => cfg.background_color || defaultConfig.background_color,
                set: (v) => { cfg.background_color = v; window.elementSdk.setConfig({ background_color: v }); }
              },
              {
                get: () => cfg.surface_color || defaultConfig.surface_color,
                set: (v) => { cfg.surface_color = v; window.elementSdk.setConfig({ surface_color: v }); }
              },
              {
                get: () => cfg.text_color || defaultConfig.text_color,
                set: (v) => { cfg.text_color = v; window.elementSdk.setConfig({ text_color: v }); }
              },
              {
                get: () => cfg.primary_action_color || defaultConfig.primary_action_color,
                set: (v) => { cfg.primary_action_color = v; window.elementSdk.setConfig({ primary_action_color: v }); }
              },
              {
                get: () => cfg.secondary_action_color || defaultConfig.secondary_action_color,
                set: (v) => { cfg.secondary_action_color = v; window.elementSdk.setConfig({ secondary_action_color: v }); }
              }
            ],
            borderables: [],
            fontEditable: undefined,
            fontSizeable: undefined
          }),
          mapToEditPanelValues: (cfg) => new Map([
            ['app_title', cfg.app_title || defaultConfig.app_title],
            ['tagline', cfg.tagline || defaultConfig.tagline]
          ])
        });
      }
    }

    // Initialize app
    async function init() {
      // Initialize Element SDK
      await initElementSdk();
      applyConfig();
      
      // Initialize Data SDK
      if (window.dataSdk) {
        const result = await window.dataSdk.init(dataHandler);
        if (!result.isOk) {
          console.error('Failed to initialize Data SDK');
        }
      }
      
      // Event listeners
      document.getElementById('workload-form').addEventListener('submit', handleFormSubmit);
      document.getElementById('accept-optimization').addEventListener('click', acceptOptimization);
    }

    init();
  </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9cd50354c4767edf',t:'MTc3MDk5MjkxNS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>