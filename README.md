```html
<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>เที่ยวระยอง ลองแล้วจะรัก | Rayong Travel Guide</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Chakra Petch & Sarabun -->
    <link href="https://fonts.googleapis.com/css2?family=Chakra+Petch:wght@400;600;700&family=Sarabun:wght@300;400;600;700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Sarabun', 'sans-serif'],
                        heading: ['Chakra Petch', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        .hero-bg {
            background-image: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 font-sans">

    <!-- Navbar -->
    <nav class="bg-white/95 backdrop-blur-md shadow-sm sticky top-0 z-50 transition-all">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">
                    <span class="font-heading text-2xl font-bold text-emerald-600 tracking-wide flex items-center gap-2">
                        <i class="fa-solid fa-umbrella-beach"></i> RAYONG GO
                    </span>
                </div>
                <div class="hidden md:flex items-center space-x-8 text-sm font-semibold">
                    <a href="#hero" class="text-slate-600 hover:text-emerald-600 transition">หน้าแรก</a>
                    <a href="#destinations" class="text-slate-600 hover:text-emerald-600 transition">สถานที่ท่องเที่ยว</a>
                    <a href="#planner" class="text-slate-600 hover:text-emerald-600 transition">จัดทริปเที่ยว</a>
                    <a href="#tips" class="text-slate-600 hover:text-emerald-600 transition">ข้อมูลการเดินทาง</a>
                </div>
                <!-- Mobile menu button -->
                <div class="flex items-center md:hidden">
                    <button onclick="toggleMobileMenu()" class="text-slate-600 hover:text-slate-900 focus:outline-none">
                        <i class="fa-solid fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-slate-100 px-4 pt-2 pb-4 space-y-1">
            <a href="#hero" onclick="toggleMobileMenu()" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">หน้าแรก</a>
            <a href="#destinations" onclick="toggleMobileMenu()" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">สถานที่ท่องเที่ยว</a>
            <a href="#planner" onclick="toggleMobileMenu()" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">จัดทริปเที่ยว</a>
            <a href="#tips" onclick="toggleMobileMenu()" class="block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">ข้อมูลการเดินทาง</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <header id="hero" class="hero-bg h-[500px] flex items-center justify-center text-center px-4">
        <div class="max-w-3xl text-white">
            <span class="bg-emerald-500/90 text-xs uppercase tracking-widest px-3 py-1 rounded-full font-bold">ระยอง... สวรรค์ของคนรักทะเลและธรรมชาติ</span>
            <h1 class="font-heading text-4xl sm:text-6xl font-bold mt-4 mb-6 drop-shadow-md">เที่ยวระยอง ลองแล้วจะรัก</h1>
            <p class="text-lg sm:text-xl mb-8 text-slate-200 drop-shadow-sm font-light">สัมผัสทะเลสวย เกาะสวรรค์ ทุ่งไม้สีทองอร่าม และอาหารทะเลสดๆ ที่รอให้คุณมาพิสูจน์ได้ทุกวัน</p>
            <a href="#destinations" class="bg-emerald-600 hover:bg-emerald-500 text-white font-bold px-8 py-3.5 rounded-full shadow-lg transition duration-300">
                สำรวจสถานที่ท่องเที่ยว <i class="fa-solid fa-arrow-down ml-2"></i>
            </a>
        </div>
    </header>

    <!-- Travel Stats Section -->
    <section class="max-w-6xl mx-auto -mt-12 px-4 relative z-10">
        <div class="bg-white rounded-2xl shadow-xl p-6 sm:p-8 grid grid-cols-2 md:grid-cols-4 gap-6 text-center border border-slate-100">
            <div>
                <p class="text-3xl font-heading font-bold text-emerald-600">3</p>
                <p class="text-xs text-slate-500 mt-1">ชั่วโมงจากกรุงเทพฯ</p>
            </div>
            <div class="border-l border-slate-100">
                <p class="text-3xl font-heading font-bold text-emerald-600">100+</p>
                <p class="text-xs text-slate-500 mt-1">กิโลเมตรแนวชายฝั่ง</p>
            </div>
            <div class="border-l border-slate-100">
                <p class="text-3xl font-heading font-bold text-emerald-600">14</p>
                <p class="text-xs text-slate-500 mt-1">เกาะสวยงามน่าค้นหา</p>
            </div>
            <div class="border-l border-slate-100">
                <p class="text-3xl font-heading font-bold text-emerald-600">365</p>
                <p class="text-xs text-slate-500 mt-1">วัน เที่ยวได้ตลอดปี</p>
            </div>
        </div>
    </section>

    <!-- Destinations Section -->
    <section id="destinations" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
        <div class="text-center mb-12">
            <h2 class="font-heading text-3xl sm:text-4xl font-bold text-slate-900 mb-4">จุดปักหมุดยอดฮิตในระยอง</h2>
            <p class="text-slate-600 max-w-2xl mx-auto">เราได้คัดสรรสุดยอดสถานที่ท่องเที่ยวหลากหลายสไตล์ เพื่อตอบโจทย์ทุกความชอบของคุณ</p>
            
            <!-- Category Tabs -->
            <div class="flex flex-wrap justify-center gap-2 mt-8">
                <button onclick="filterCategory('all')" class="category-btn active px-5 py-2 rounded-full text-sm font-semibold border transition duration-300 bg-emerald-600 text-white border-emerald-600" id="btn-all">
                    ทั้งหมด
                </button>
                <button onclick="filterCategory('beach')" class="category-btn px-5 py-2 rounded-full text-sm font-semibold border transition duration-300 bg-white text-slate-600 border-slate-200 hover:border-emerald-600 hover:text-emerald-600" id="btn-beach">
                    <i class="fa-solid fa-water-wave mr-1"></i> ทะเล & เกาะ
                </button>
                <button onclick="filterCategory('nature')" class="category-btn px-5 py-2 rounded-full text-sm font-semibold border transition duration-300 bg-white text-slate-600 border-slate-200 hover:border-emerald-600 hover:text-emerald-600" id="btn-nature">
                    <i class="fa-solid fa-tree mr-1"></i> ป่าไม้ & ธรรมชาติ
                </button>
                <button onclick="filterCategory('culture')" class="category-btn px-5 py-2 rounded-full text-sm font-semibold border transition duration-300 bg-white text-slate-600 border-slate-200 hover:border-emerald-600 hover:text-emerald-600" id="btn-culture">
                    <i class="fa-solid fa-landmark mr-1"></i> วัฒนธรรม & ประวัติศาสตร์
                </button>
                <button onclick="filterCategory('cafe')" class="category-btn px-5 py-2 rounded-full text-sm font-semibold border transition duration-300 bg-white text-slate-600 border-slate-200 hover:border-emerald-600 hover:text-emerald-600" id="btn-cafe">
                    <i class="fa-solid fa-mug-saucer mr-1"></i> คาเฟ่ & จุดแชะภาพ
                </button>
            </div>
        </div>

        <!-- Destination Cards Grid -->
        <div id="destinations-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Dynamic Cards Load via JS -->
        </div>
    </section>

    <!-- Interactive Trip Planner Section -->
    <section id="planner" class="bg-slate-900 text-white py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div>
                    <span class="text-emerald-400 font-bold uppercase tracking-wider text-xs">Easy Trip Planner</span>
                    <h2 class="font-heading text-3xl sm:text-4xl font-bold mt-2 mb-6">ออกแบบแผนเที่ยวระยองง่ายๆ ใน 1 นาที</h2>
                    <p class="text-slate-400 mb-8">เพียงเลือกสถานที่ที่คุณสนใจด้านล่าง ระบบจะจัดลำดับและสร้างเส้นทางท่องเที่ยวเบื้องต้นที่เหมาะสำหรับคุณทันที!</p>
                    
                    <div class="space-y-4">
                        <label class="block text-sm font-medium text-slate-300">เลือกจุดท่องเที่ยวที่อยากไป (เลือกได้หลายแห่ง):</label>
                        <div id="planner-checkboxes" class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                            <!-- Injected by JS -->
                        </div>
                        <button onclick="generateTripPlan()" class="w-full sm:w-auto bg-emerald-600 hover:bg-emerald-500 text-white font-bold px-8 py-3.5 rounded-xl shadow-lg transition mt-4">
                            สร้างแผนท่องเที่ยวจำลอง
                        </button>
                    </div>
                </div>

                <div class="bg-slate-800 border border-slate-700 rounded-2xl p-6 sm:p-8">
                    <div class="flex items-center justify-between border-b border-slate-700 pb-4 mb-6">
                        <h3 class="font-heading text-xl font-bold text-emerald-400"><i class="fa-solid fa-route mr-2"></i> แผนการเดินทางของคุณ</h3>
                        <span id="trip-days" class="bg-emerald-950 text-emerald-400 border border-emerald-900 px-3 py-1 rounded-full text-xs font-bold">1 วัน</span>
                    </div>
                    
                    <div id="trip-result" class="space-y-6">
                        <div class="text-center text-slate-500 py-12">
                            <i class="fa-solid fa-map-location-dot text-4xl mb-3 block text-slate-600"></i>
                            <p>กรุณาเลือกสถานที่ท่องเที่ยวซ้ายมือเพื่อประกอบแผนการเดินทาง</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Travel Tips Section -->
    <section id="tips" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
        <div class="text-center mb-12">
            <h2 class="font-heading text-3xl sm:text-4xl font-bold text-slate-900 mb-4">ข้อมูลพกเป้สำหรับเที่ยวระยอง</h2>
            <p class="text-slate-600 max-w-2xl mx-auto">คำถามพบบ่อยและข้อแนะนำสำหรับการเดินทางไปเที่ยวระยองให้อิ่มหนำสำราญใจ</p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div class="bg-white p-6 rounded-2xl border border-slate-100 shadow-sm">
                <div class="w-12 h-12 rounded-xl bg-emerald-50 text-emerald-600 flex items-center justify-center text-xl mb-4">
                    <i class="fa-solid fa-car"></i>
                </div>
                <h3 class="font-heading text-lg font-bold text-slate-900 mb-2">การเดินทาง</h3>
                <p class="text-sm text-slate-600 leading-relaxed">
                    ขับรถจากกรุงเทพฯ ใช้เส้นทางมอเตอร์เวย์สาย 7 ต่อเนื่องด้วยทางหลวงหมายเลข 36 หรือ 344 ใช้เวลาประมาณ 2.5 - 3 ชั่วโมง นอกจากนี้ยังมีรถตู้โดยสารสาธารณะบริการจากเอกมัยและหมอชิต 2 สู่ตัวเมืองระยองและบ้านเพทุกวัน
                </p>
            </div>
            <div class="bg-white p-6 rounded-2xl border border-slate-100 shadow-sm">
                <div class="w-12 h-12 rounded-xl bg-emerald-50 text-emerald-600 flex items-center justify-center text-xl mb-4">
                    <i class="fa-solid fa-calendar-days"></i>
                </div>
                <h3 class="font-heading text-lg font-bold text-slate-900 mb-2">เที่ยวช่วงไหนดี?</h3>
                <p class="text-sm text-slate-600 leading-relaxed">
                    <strong>พฤศจิกายน - เมษายน:</strong> เหมาะสำหรับการเที่ยวทะเล เกาะเสม็ด ลมสงบ น้ำใสแจ๋ว <br>
                    <strong>พฤษภาคม - กรกฎาคม:</strong> เทศกาลผลไม้รสล้ำ เงาะ ทุเรียน มังคุด สดๆ จากสวนระยองแท้ๆ
                </p>
            </div>
            <div class="bg-white p-6 rounded-2xl border border-slate-100 shadow-sm">
                <div class="w-12 h-12 rounded-xl bg-emerald-50 text-emerald-600 flex items-center justify-center text-xl mb-4">
                    <i class="fa-solid fa-fish"></i>
                </div>
                <h3 class="font-heading text-lg font-bold text-slate-900 mb-2">ของฝากห้ามพลาด</h3>
                <p class="text-sm text-slate-600 leading-relaxed">
                    มาถึงระยองต้องไม่พลาดซื้อ น้ำปลาแท้ระยอง, กะปิหวานบ้านเพ, ทุเรียนทอด, ปลาหมึกแห้งแปรรูป และผลไม้สดๆ จากสวนผลไม้ท้องถิ่นซึ่งมีราคาย่อมเยาและคุณภาพเยี่ยมยอด
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-slate-950 text-slate-400 py-12 border-t border-slate-900">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h3 class="font-heading text-2xl font-bold text-white mb-4">เที่ยวระยอง ลองแล้วจะรัก</h3>
            <p class="text-sm text-slate-500 max-w-md mx-auto mb-8">เว็บแอปพลิเคชันแนะนำสถานที่ท่องเที่ยวจังหวัดระยอง รวดเร็ว ปลอดภัย และอัปเดตข้อมูลการเดินทางเพื่อคุณ</p>
            <div class="flex justify-center space-x-6 mb-8 text-lg">
                <a href="#" class="hover:text-emerald-400 transition"><i class="fa-brands fa-facebook"></i></a>
                <a href="#" class="hover:text-emerald-400 transition"><i class="fa-brands fa-instagram"></i></a>
                <a href="#" class="hover:text-emerald-400 transition"><i class="fa-solid fa-envelope"></i></a>
            </div>
            <p class="text-xs text-slate-600">&copy; 2026 Rayong Go Travel Guide. สงวนลิขสิทธิ์ทั้งหมด</p>
        </div>
    </footer>

    <!-- Place Details Modal (Hidden Initially) -->
    <div id="details-modal" class="hidden fixed inset-0 z-[100] flex items-center justify-center p-4 bg-slate-950/80 backdrop-blur-sm">
        <div class="bg-white rounded-2xl max-w-2xl w-full p-6 text-slate-900 shadow-2xl relative">
            <button onclick="closeModal()" class="absolute top-4 right-4 text-slate-400 hover:text-slate-600">
                <i class="fa-solid fa-circle-xmark text-2xl"></i>
            </button>
            <div id="modal-content">
                <!-- Injected via JS -->
            </div>
        </div>
    </div>

    <script>
        // Destinations Data Pool
        const destinations = [
            {
                id: "samet",
                name: "เกาะเสม็ด",
                category: "beach",
                summary: "เกาะสวรรค์แห่งทะเลตะวันออกที่มีหาดทรายขาวเนียนละเอียดดั่งแป้ง",
                desc: "เกาะเสม็ดคือจุดหมายปลายทางยอดฮิตระดับโลก โดดเด่นด้วยเม็ดทรายสีขาวเนียนละเอียดตลอดแนวชายหาด มีหาดชื่อดังมากมาย เช่น หาดทรายแก้ว อ่าววงเดือน และอ่าวประการัง เหมาะสำหรับกิจกรรมดำน้ำ ดูปะการัง และปาร์ตี้ริมหาดยามค่ำคืน",
                img: "https://images.unsplash.com/photo-1544735716-392fe2489ffa?auto=format&fit=crop&w=600&q=80",
                location: "ต.เพ อ.เมืองระยอง",
                highlight: "ชมการแสดงควงกระบองไฟที่อ่าวไผ่หรือหาดทรายแก้วยามค่ำคืน"
            },
            {
                id: "tungprongtong",
                name: "ทุ่งโปรงทอง",
                category: "nature",
                summary: "ทุ่งต้นโปรงสีเหลืองทองกว้างใหญ่ริมปากน้ำประแส",
                desc: "ทุ่งโปรงทองเป็นแหล่งท่องเที่ยวเชิงอนุรักษ์ธรรมชาติ มีสะพานไม้ทอดยาวกว่า 2 กิโลเมตรให้เดินชมธรรมชาติป่าชายเลน ท่ามกลางต้นโปรงทองที่ขึ้นหนาแน่น เมื่อแสงแดดส่องกระทบจะสะท้อนสีทองอร่ามงดงามตระการตา",
                img: "https://images.unsplash.com/photo-1513836279014-a89f7a76ae86?auto=format&fit=crop&w=600&q=80",
                location: "ปากน้ำประแส อ.แกลง",
                highlight: "ถ่ายภาพมุมกว้างแบบพาโนรามา ณ จุดชมวิวทุ่งสะท้อนสีทองอร่าม"
            },
            {
                id: "yomjinda",
                name: "ถนนยมจินดา",
                category: "culture",
                summary: "ย้อนวันวานย่านเมืองเก่าระยอง อบอวลด้วยเสน่ห์สถาปัตยกรรมคลาสสิก",
                desc: "ถนนยมจินดาเป็นถนนสายแรกของเมืองระยอง ปัจจุบันได้รับการอนุรักษ์อาคารบ้านไม้เก่าแก่สไตล์สากล-จีนโบราณ มีร้านขายของย้อนยุค พิพิธภัณฑ์เมืองระยอง และร้านอาหารท้องถิ่นรสชาติดั้งเดิมมากมาย",
                img: "https://images.unsplash.com/photo-1473163928189-364b2c4e1135?auto=format&fit=crop&w=600&q=80",
                location: "ต.ท่าประดู่ อ.เมืองระยอง",
                highlight: "ลิ้มลองก๋วยเตี๋ยวโบราณและกาแฟสไตล์สภากาแฟย้อนยุค"
            },
            {
                id: "aquarium",
                name: "สถานแสดงพันธุ์สัตว์น้ำระยอง",
                category: "nature",
                summary: "อุโมงค์ปลาใต้น้ำเพื่อเรียนรู้วิถีชีวิตสัตว์ทะเลอย่างใกล้ชิด",
                desc: "ศูนย์วิจัยและพัฒนาประมงทะเลชายฝั่ง จัดแสดงสัตว์น้ำจืดและน้ำเค็มสายพันธุ์ต่างๆ มีไฮไลท์อยู่ที่อุโมงค์กระจกทางเดินใสที่ให้ความรู้สึกเสมือนกำลังเดินอยู่ใต้ท้องทะเลลึก เหมาะสำหรับการมาทัศนศึกษาเป็นครอบครัว",
                img: "https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=600&q=80",
                location: "ต.เพ อ.เมืองระยอง",
                highlight: "เดินชมอุโมงค์ปลาทะเลขนาดใหญ่พร้อมสัมผัสบ่อสัตว์ทะเลแบบ Touch Pool"
            },
            {
                id: "khaochamao",
                name: "อุทยานแห่งชาติน้ำตกเขาชะเมา-เขาวง",
                category: "nature",
                summary: "น้ำตกใสไหลเย็นเจ็ดชั้นท่ามกลางป่าอุดมสมบูรณ์",
                desc: "ผืนป่าที่อุดมสมบูรณ์และเป็นแหล่งต้นน้ำลำธาร จุดเด่นคือน้ำตกเขาชะเมาที่มีน้ำใสสะอาดจนสามารถมองเห็นฝูงปลาพลวงพริ้วไหวใต้น้ำ มีทั้งหมด 7 ชั้น และยังมีจุดท่องเที่ยวถ้ำเขาวงที่ซ่อนตัวอยู่ไม่ไกล",
                img: "https://images.unsplash.com/photo-1441974231531-c6227db76b6e?auto=format&fit=crop&w=600&q=80",
                location: "อ.เขาชะเมา",
                highlight: "นั่งพักผ่อนชมฝูงปลาพลวงจำนวนมากที่แหวกว่ายบริเวณชั้น 'วังมัจฉา'"
            },
            {
                id: "straycafe",
                name: "จุดชมวิวเนินนางพญา & หาดแสงจันทร์",
                category: "cafe",
                summary: "ถนนเลียบหาดรูปพระจันทร์เสี้ยวที่สวยแปลกตาไม่ซ้ำใคร",
                desc: "หาดแสงจันทร์เป็นชายหาดที่มีแนวหินกั้นคลื่นลมสร้างลักษณะเว้าแหว่งคล้ายรูปพระจันทร์ครึ่งเสี้ยวเรียงรายเป็นแนวยาว เป็นจุดแคมป์ปิ้งและคาเฟ่ยอดฮิต มีมุมสวยๆ ถ่ายภาพริมชายฝั่งทะเลระยองที่งดงามแปลกตา",
                img: "https://images.unsplash.com/photo-1505118380757-91f5f5632de0?auto=format&fit=crop&w=600&q=80",
                location: "อ.เมืองระยอง",
                highlight: "ขับรถชมวิวเลียบหาดยามอาทิตย์อัสดง"
            }
        ];

        // Mobile Menu Control
        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        }

        // Render Destinations
        function renderDestinations(items) {
            const grid = document.getElementById('destinations-grid');
            grid.innerHTML = '';

            items.forEach(item => {
                const card = document.createElement('div');
                card.className = "bg-white rounded-2xl overflow-hidden shadow-sm hover:shadow-xl transition duration-300 border border-slate-100 flex flex-col justify-between";
                
                let categoryLabel = "";
                let categoryColor = "";
                
                switch(item.category) {
                    case 'beac# Kk
