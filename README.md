<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CJ RESALES | Premium Supply</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;800&display=swap" rel="stylesheet">
    <style>
        body { 
            font-family: 'Plus Jakarta Sans', sans-serif; 
            background-color: #050505; 
            color: white; 
            overflow-x: hidden; 
        }
        .glass { 
            background: rgba(255, 255, 255, 0.03); 
            backdrop-filter: blur(12px); 
            border: 1px solid rgba(255, 255, 255, 0.08); 
        }
        .product-card:hover .product-image { 
            transform: scale(1.08); 
        }
        .custom-scrollbar::-webkit-scrollbar { width: 4px; }
        .custom-scrollbar::-webkit-scrollbar-thumb { 
            background: #4f46e5; 
            border-radius: 10px; 
        }
    </style>
</head>
<body>

    <nav class="fixed top-0 w-full z-[100] glass border-b border-white/5">
        <div class="max-w-7xl mx-auto px-6 py-5 flex justify-between items-center">
            <div class="flex items-center gap-2">
                <div class="w-8 h-8 bg-indigo-600 rounded-lg flex items-center justify-center font-black italic">CJ</div>
                <h1 class="text-xl font-extrabold tracking-tighter uppercase">RESALES</h1>
            </div>
            
            <div class="flex items-center gap-6">
                <button onclick="showOrders()" 
                        class="text-xs font-bold uppercase tracking-widest px-4 py-2 hover:bg-white/5 rounded-full transition">
                    VIEW ORDERS
                </button>
                <button onclick="toggleCart()" class="relative p-2 hover:bg-white/5 rounded-full transition">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 11V7a4 4 0 00-8 0v4M5 9h14l1 12H4L5 9z" />
                    </svg>
                    <span id="cart-count" class="absolute -top-1 -right-1 bg-indigo-600 text-[10px] font-black w-5 h-5 flex items-center justify-center rounded-full border-2 border-black">0</span>
                </button>
            </div>
        </div>
    </nav>

    <main class="max-w-7xl mx-auto px-6 pt-44 grid grid-cols-1 md:grid-cols-3 gap-12 mb-24">
        
        <!-- 1. Essentials Hoodie -->
        <div class="product-card group">
            <div class="relative aspect-[3/4] overflow-hidden rounded-[2.5rem] bg-zinc-900 border border-white/10">
                <img src="https://i.imgur.com/NXhRJ.jpg" 
                     alt="Essentials Hoodie"
                     class="product-image w-full h-full object-cover opacity-70 group-hover:opacity-100 transition-all duration-700">
                <div class="absolute inset-0 bg-gradient-to-t from-black via-transparent p-8 flex flex-col justify-end opacity-0 group-hover:opacity-100 transition-all">
                    <button onclick="addToCart('Essentials Hoodie', 35.00, 'Small')" 
                            class="bg-white text-black font-black py-4 rounded-2xl hover:bg-indigo-600 hover:text-white transition transform translate-y-4 group-hover:translate-y-0 duration-300">
                        QUICK ADD
                    </button>
                </div>
            </div>
            <div class="mt-6 flex justify-between items-center px-2">
                <div>
                    <h4 class="font-bold uppercase italic tracking-tighter text-xl leading-none">Essentials Hoodie</h4>
                    <p class="text-indigo-500 text-xs font-bold mt-2 uppercase">Small (Fits Big)</p>
                </div>
                <p class="text-2xl font-black">$35</p>
            </div>
        </div>

        <!-- 2. RL Chaps Hoodie -->
        <div class="product-card group">
            <div class="relative aspect-[3/4] overflow-hidden rounded-[2.5rem] bg-zinc-900 border border-white/10">
                <img src="https://i.imgur.com/tASNJ.jpg" 
                     alt="RL Chaps Hoodie"
                     class="product-image w-full h-full object-cover opacity-70 group-hover:opacity-100 transition-all duration-700">
                <div class="absolute inset-0 bg-gradient-to-t from-black via-transparent p-8 flex flex-col justify-end opacity-0 group-hover:opacity-100 transition-all">
                    <button onclick="addToCart('RL Chaps Hoodie', 45.00, 'L')" 
                            class="bg-white text-black font-black py-4 rounded-2xl hover:bg-indigo-600 hover:text-white transition transform translate-y-4 group-hover:translate-y-0 duration-300">
                        QUICK ADD
                    </button>
                </div>
            </div>
            <div class="mt-6 flex justify-between items-center px-2">
                <div>
                    <h4 class="font-bold uppercase italic tracking-tighter text-xl leading-none">RL Chaps Hoodie</h4>
                    <p class="text-zinc-500 text-xs font-bold mt-2 uppercase">Vintage Selection</p>
                </div>
                <p class="text-2xl font-black">$45</p>
            </div>
        </div>

        <!-- 3. Travis Scott's Shoes - Updated with your new photo -->
        <div class="product-card group">
            <div class="relative aspect-[3/4] overflow-hidden rounded-[2.5rem] bg-zinc-900 border border-white/10">
                <img src="https://i.imgur.com/xCq9d.jpg" 
                     alt="Travis Scott's"
                     class="product-image w-full h-full object-cover opacity-70 group-hover:opacity-100 transition-all duration-700">
                <div class="absolute inset-0 bg-gradient-to-t from-black via-transparent p-8 flex flex-col justify-end opacity-0 group-hover:opacity-100 transition-all">
                    <button onclick="addToCart('Travis Scott\'s', 150.00, '8.5')" 
                            class="bg-white text-black font-black py-4 rounded-2xl hover:bg-indigo-600 hover:text-white transition transform translate-y-4 group-hover:translate-y-0 duration-300">
                        QUICK ADD
                    </button>
                </div>
            </div>
            <div class="mt-6 flex justify-between items-center px-2">
                <div>
                    <h4 class="font-bold uppercase italic tracking-tighter text-xl leading-none">Travis Scott's</h4>
                    <p class="text-indigo-500 text-xs font-bold mt-2 uppercase">Size 8.5</p>
                </div>
                <p class="text-2xl font-black">$150</p>
            </div>
        </div>
    </main>

    <!-- Cart Sidebar -->
    <div id="cart-sidebar" class="fixed top-0 right-0 h-full w-full md:w-[450px] glass z-[1000] transform translate-x-full transition-transform duration-500 p-10 flex flex-col border-l border-white/10 shadow-2xl">
        <div class="flex justify-between items-center mb-10">
            <h2 class="text-4xl font-black italic uppercase tracking-tighter">Bag</h2>
            <button onclick="toggleCart()" class="text-zinc-500 hover:text-white text-5xl font-light">&times;</button>
        </div>
        <div id="cart-items" class="flex-1 overflow-y-auto space-y-6 custom-scrollbar pr-2"></div>
        <div class="pt-8 border-t border-white/10 mt-8">
            <div class="flex justify-between items-end mb-8">
                <span class="text-zinc-500 font-bold uppercase tracking-widest text-[10px]">Subtotal</span>
                <span id="cart-total" class="text-4xl font-black italic tracking-tighter text-indigo-500">$0.00</span>
            </div>
            <button onclick="checkout()" 
                    class="w-full bg-[#00D632] hover:bg-[#00c22d] text-white py-6 rounded-3xl font-black text-xl flex items-center justify-center gap-4 transition-all shadow-lg shadow-green-500/20">
                PAY VIA CASH APP
            </button>
        </div>
    </div>

    <!-- Orders Modal -->
    <div id="orders-modal" class="hidden fixed inset-0 bg-black/80 z-[2000] flex items-center justify-center">
        <div class="glass w-full max-w-2xl mx-4 rounded-3xl p-8 max-h-[90vh] overflow-hidden flex flex-col">
            <div class="flex justify-between items-center mb-6">
                <h2 class="text-3xl font-black italic uppercase tracking-tighter">Recent Orders</h2>
                <button onclick="hideOrders()" class="text-4xl leading-none text-zinc-400 hover:text-white">&times;</button>
            </div>
            <div id="orders-list" class="flex-1 overflow-y-auto custom-scrollbar pr-2 space-y-4 text-sm"></div>
            <button onclick="clearOrders()" 
                    class="mt-6 text-red-400 hover:text-red-500 text-xs font-bold uppercase tracking-widest">
                Clear All Orders
            </button>
        </div>
    </div>

    <script>
        const myCashTag = "carterbarrels"; 
        let cart = [];
        let orders = JSON.parse(localStorage.getItem('cjresales_orders')) || [];

        function toggleCart() {
            const sidebar = document.getElementById('cart-sidebar');
            sidebar.classList.toggle('translate-x-full');
        }

        function addToCart(name, price, size) {
            const existing = cart.find(item => item.name === name && item.size === size);
            if (existing) existing.qty++;
            else cart.push({ name, price, size, qty: 1 });
            updateCartUI();
            const sidebar = document.getElementById('cart-sidebar');
            if (sidebar.classList.contains('translate-x-full')) toggleCart();
        }

        function removeFromCart(name) {
            cart = cart.filter(item => item.name !== name);
            updateCartUI();
        }

        function updateCartUI() {
            const container = document.getElementById('cart-items');
            const totalCount = cart.reduce((sum, item) => sum + item.qty, 0);
            document.getElementById('cart-count').innerText = totalCount;
            
            if (cart.length === 0) {
                container.innerHTML = '<p class="text-zinc-700 font-bold uppercase italic mt-10 text-center">Your bag is empty.</p>';
                document.getElementById('cart-total').innerText = "$0.00";
                return;
            }

            let total = 0;
            container.innerHTML = cart.map((item) => {
                total += (item.price * item.qty);
                return `
                    <div class="flex justify-between items-center bg-white/5 p-4 rounded-2xl border border-white/5">
                        <div>
                            <h4 class="font-black uppercase italic tracking-tighter text-lg leading-tight">${item.name}</h4>
                            <p class="text-indigo-400 font-bold text-[10px] mt-1 uppercase">SIZE ${item.size} — x${item.qty}</p>
                        </div>
                        <div class="text-right">
                            <p class="text-xl font-black tracking-tighter">$${(item.price * item.qty).toFixed(2)}</p>
                            <button onclick="removeFromCart('${item.name}')" class="text-red-500 text-[10px] font-black uppercase mt-1">Remove</button>
                        </div>
                    </div>
                `;
            }).join('');
            document.getElementById('cart-total').innerText = `$${total.toFixed(2)}`;
        }

        function checkout() {
            if (cart.length === 0) return;
            
            const total = cart.reduce((sum, item) => sum + (item.price * item.qty), 0);
            const summary = cart.map(i => `${i.qty}x ${i.name} (${i.size})`).join(', ');
            
            const order = {
                id: Date.now(),
                date: new Date().toLocaleString(),
                total: total.toFixed(2),
                summary: summary
            };
            
            orders.unshift(order);
            localStorage.setItem('cjresales_orders', JSON.stringify(orders));
            
            const note = encodeURIComponent(`CJ Resales Order: ${summary}`);
            window.location.href = `https://cash.app/$${myCashTag}/${total.toFixed(2)}?note=${note}`;
            
            setTimeout(() => {
                cart = [];
                updateCartUI();
            }, 500);
        }

        function showOrders() {
            const modal = document.getElementById('orders-modal');
            const list = document.getElementById('orders-list');
            
            list.innerHTML = orders.length === 0 
                ? `<p class="text-zinc-500 italic text-center py-10">No orders yet...</p>`
                : orders.map(order => `
                    <div class="bg-white/5 p-5 rounded-2xl border border-white/10">
                        <div class="flex justify-between text-xs text-zinc-400 mb-2">
                            <span>${order.date}</span>
                            <span class="font-mono">$${order.total}</span>
                        </div>
                        <p class="font-medium">${order.summary}</p>
                    </div>
                `).join('');
            
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function hideOrders() {
            const modal = document.getElementById('orders-modal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        function clearOrders() {
            if (confirm("Clear ALL saved orders?")) {
                orders = [];
                localStorage.setItem('cjresales_orders', JSON.stringify(orders));
                hideOrders();
            }
        }

        document.getElementById('orders-modal').addEventListener('click', function(e) {
            if (e.target === this) hideOrders();
        });
    </script>
</body>
</html>
