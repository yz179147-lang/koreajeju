<!-- Chosen Palette: Warm Neutrals (Background: bg-orange-50, Cards: bg-white, Accents: text-orange-600) -->
<!DOCTYPE html>
<html lang="zh-Hant" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🎂 ㄅㄅㄐ公主生日 濟州之旅</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Inter', 'Noto Sans TC', sans-serif;
            background-color: #fffaf0; 
        }
        .nav-link {
            @apply px-3 py-2 text-sm md:px-4 md:text-base font-medium text-gray-600 bg-white hover:bg-gray-50 rounded-lg shadow-md border border-gray-300 transition-all duration-200;
        }
        .nav-link.active {
            @apply bg-orange-600 text-white font-semibold border-orange-600 shadow-lg;
        }
        .itinerary-card {
            @apply bg-white rounded-xl shadow-lg overflow-hidden transition-all duration-300 hover:shadow-xl;
        }
    </style>
</head>
<body class="text-gray-800">

    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-white/90 backdrop-blur-md shadow-md">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row md:items-center md:justify-between py-2">
                <h1 class="text-xl md:text-2xl font-bold text-orange-600 text-center md:text-left py-2">🎂 ㄅㄅㄐ公主生日之旅</h1>
                <!-- Navigation replaced with Select Dropdown -->
                <div class="relative mt-2 md:mt-0">
                    <select id="navigation-select" class="w-full md:w-auto appearance-none px-4 py-2 text-base font-medium text-gray-700 bg-white rounded-lg shadow-md border border-gray-300 focus:outline-none focus:ring-2 focus:ring-orange-500 focus:border-orange-500">
                        <option value="all">全部顯示</option>
                        <option value="#section-tips">行前提醒</option>
                        <option value="#section-day1">Day 1 (11/30)</option>
                        <option value="#section-day2">Day 2 (12/1)</option>
                        <option value="#section-day3">Day 3 (12/2)</option>
                        <option value="#section-day4">Day 4 (12/3)</option>
                    </select>
                    <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700">
                        <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- Main Content Area -->
    <main class="container mx-auto p-4 md:p-8" id="app-content">

        <!-- Section: Pre-trip Tips -->
        <section id="section-tips" class="mb-12 pt-16 -mt-16">
            <h2 class="text-3xl font-bold text-gray-900 mb-6 border-b-2 border-orange-200 pb-2">⚠️ 在地人行前貼心提醒</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <div class="bg-white p-6 rounded-xl shadow-lg">
                    <ul class="space-y-4">
                        <li class="flex items-start">
                            <span class="text-2xl mr-3">🌡️</span>
                            <div><strong class="text-orange-700">天氣 (11/30-12/03)</strong>：濟州初冬，氣溫約 5°C - 12°C。**風非常大**，體感溫度更低。請務必攜帶防風外套、羽絨衣、毛帽和暖暖包。</div>
                        </li>
                        <li class="flex items-start">
                            <span class="text-2xl mr-3">🌇</span>
                            <div><strong class="text-orange-700">日落時間</strong>：冬季日落早（約 17:20），郊區天黑後路燈很少，建議 17:00 前結束戶外景點。</div>
                        </li>
                        <li class="flex items-start">
                            <span class="text-2xl mr-3">🗺️</span>
                            <div><strong class="text-orange-700">導航 App</strong>：Google Maps 在韓國無法導航。請務必下載 **Naver Map** 或 **Kakao Map**。您可以使用本文件中的「韓文名稱」或「電話號碼」來搜尋。</div>
                        </li>
                        <li class="flex items-start">
                            <span class="text-2xl mr-3">🚗</span>
                            <div><strong class="text-orange-700">租車</strong>：請備妥「**護照、台灣駕照正本、有效國際駕照**」，三者缺一不可。</div>
                        </li>
                        <li class="flex items-start">
                            <span class="text-2xl mr-3">🔌</span>
                            <div><strong class="text-orange-700">電壓</strong>：韓國電壓為 220V，插座為兩腳圓形（德規），請攜帶轉接頭。</div>
                        </li>
                    </ul>
                </div>
                
                <div class="bg-white p-6 rounded-xl shadow-lg">
                    <h3 class="text-2xl font-semibold text-gray-900 mb-4">🏨 您的住宿資訊</h3>
                    <dl class="space-y-3">
                        <div>
                            <dt class="font-semibold text-orange-700">飯店名稱</dt>
                            <dd class="text-gray-700">Sea Stay Hotel (씨스테이호텔)</dd>
                        </div>
                        <div>
                            <dt class="font-semibold text-orange-700">地址</dt>
                            <dd class="text-gray-700">제주시 애월읍 애월해안로 255</dd>
                        </div>
                        <div>
                            <dt class="font-semibold text-orange-700">電話 (導航用)</dt>
                            <dd class="text-gray-700">064-799-3660</dd>
                        </div>
                        <div>
                            <dt class="font-semibold text-orange-700">特色</dt>
                            <dd class="text-gray-700">位於涯月海岸道路核心區，所有涯月名店都在附近，房間均為海景第一排。</dd>
                        </div>
                        <div>
                            <a href="https://map.naver.com/p/search/씨스테이호텔" target="_blank" rel="noopener noreferrer" class="inline-block bg-green-500 text-white font-bold py-2 px-4 rounded-lg hover:bg-green-600 transition-colors">
                                🗺️ Naver Map 飯店位置
                            </a>
                        </div>
                    </dl>
                </div>
            </div>
        </section>

        <!-- Section: Day 1 -->
        <section id="section-day1" class="mb-12 pt-16 -mt-16">
            <h2 class="text-3xl font-bold text-gray-900 mb-2">🗓️ Day 1：抵達與黑豬肉之夜 (11/30 六)</h2>
            <p class="text-lg text-gray-600 mb-6">本日動線：機場 → 租車 → 晚餐 (老衡洞) → 入住飯店 (涯月)</p>
            <div class="space-y-6" id="day1-content"></div>
        </section>

        <!-- Section: Day 2 -->
        <section id="section-day2" class="mb-12 pt-16 -mt-16">
            <h2 class="text-3xl font-bold text-gray-900 mb-2">🗓️ Day 2：橫跨東西的長征 (12/1 日)</h2>
            <p class="text-lg text-gray-600 mb-4">本日動線：飯店 (西) → 早餐 (西) → [長途駕駛] → 東部景點 → 晚餐 (東) → [長途駕駛] → 飯店 (西)</p>
            <div class="bg-red-100 border-l-4 border-red-500 text-red-700 p-4 rounded-lg mb-6" role="alert">
                <p class="font-bold">⚠️ 關鍵提醒</p>
                <p>本日行程跨度最大。從 Saemool (西) 到 朝天窗縫岩 (東) 車程約 **1 小時**。請預留足夠交通時間。</p>
            </div>
            <div class="space-y-6" id="day2-content"></div>
        </section>

        <!-- Section: Day 3 -->
        <section id="section-day3" class="mb-12 pt-16 -mt-16">
            <h2 class="text-3xl font-bold text-gray-900 mb-2">🗓️ Day 3：西部活力與市區購物 (12/2 一)</h2>
            <p class="text-lg text-gray-600 mb-6">本日動線：飯店 (涯月) → 早午餐 (涯月) → 981 Park (涯月) → 咖啡 (涯月) → 市區購物 (濟州市)</p>
            <div class="space-y-6" id="day3-content"></div>
        </section>

        <!-- Section: Day 4 -->
        <section id="section-day4" class="pt-16 -mt-16">
            <h2 class="text-3xl font-bold text-gray-900 mb-2">🗓️ Day 4：涯月深度遊與返程 (12/3 二)</h2>
            <p class="text-lg text-gray-600 mb-6">本日動線：飯店 (涯月) → 午餐 (涯月) → 咖啡 (涯月) → 市區購物 → 機場</p>
            <div class="space-y-6" id="day4-content"></div>
        </section>

    </main>

    <footer class="text-center p-6 mt-12 bg-orange-100 text-orange-800">
        <p>祝您有趟美好的濟州之旅！</p>
        <p class="text-sm mt-1">由濟州在地嚮導「濟州人」提供支援</p>
    </footer>

    <script>
        const itineraryData = {
            day1: [
                {
                    time: "18:00",
                    title: "抵達 / 租車",
                    korean: "地點：濟州機場 (CJU)",
                    address: "接駁：Gate 5 對面「Rent-a-car House」",
                    map: "https://map.naver.com/p/search/제주국제공항",
                    tip: "落地後盡快出關，尋找您租車公司的接駁巴士。<br>💡 提醒：請再次確認接駁車最晚營運時間。"
                },
                {
                    time: "19:30",
                    title: "晚餐：熟成到 (老衡本館)",
                    korean: "숙성도 노형본관",
                    address: "제주시 원노형로 41",
                    map: "https://map.naver.com/p/search/숙성도%20노형본관",
                    tip: "您的預約店家。務必準時抵達。<br>💡 必點：您CSV中提到的「960 熟成帶骨里肌 (뼈등심)」是限量招牌。"
                },
                {
                    time: "21:30",
                    title: "入住飯店",
                    korean: "Sea Stay Hotel (씨스테이호텔)",
                    address: "제주시 애월읍 애월해안로 255",
                    map: "https://map.naver.com/p/search/씨스테이호텔",
                    tip: "從「熟成到」開車到飯店約 25 分鐘。<br>💡 提醒：飯店樓下或隔壁就有便利商店 (CU / GS25)，可購買隔日早餐或零食。"
                }
            ],
            day2: [
                {
                    time: "11:00",
                    title: "Saemool 早午餐",
                    korean: "카페 새물",
                    address: "제주시 애월읍 애월해안로 596",
                    map: "https://map.naver.com/p/search/제주새물",
                    tip: "就在您飯店附近 (車程 5 分鐘)。<br>💡 必點：Jeju Green Tangerine Tea (綠橘茶)。建議早點去搶二樓窗邊海景座位。"
                },
                {
                    time: "12:30",
                    title: "出發前往東部",
                    korean: "-",
                    address: "-",
                    map: null,
                    tip: "開始本日的長途駕駛 (約 50-60 分鐘)。"
                },
                {
                    time: "13:30",
                    title: "朝天窗縫岩",
                    korean: "창꼼바위",
                    address: "제주시 조천읍 북촌리 403-9",
                    map: "https://map.naver.com/p/search/창꼼바위",
                    tip: "《非常律師》景點。岩洞旁的停車位不多。<br>💡 提醒：海風極大，請戴好帽子和圍巾。"
                },
                {
                    time: "14:30",
                    title: "CAFE THE CONTAINER",
                    korean: "카페 더 콘테나",
                    address: "제주시 조천읍 함와로 513",
                    map: "https://map.naver.com/p/search/카페더콘테나",
                    tip: "巨大橘色籃子建築。低消一杯飲料。<br>💡 特色：飲料會用「吊籃」送下來，記得錄影！12 月是橘子季，有機會可參加採橘體驗。"
                },
                {
                    time: "16:30",
                    title: "涉地可支",
                    korean: "섭지코지",
                    address: "서귀포시 성산읍 섭지코지로 107",
                    map: "https://map.naver.com/p/search/섭지코지",
                    tip: "經典韓劇景點。走到燈塔或糖果屋即可折返。<br>💡 提醒：這裡非常空曠，風超級大。建議在此看 17:20 左右的日落，景色絕美。"
                },
                {
                    time: "18:30",
                    title: "晚餐：季節餐桌 (咸德店)",
                    korean: "계절식탁 함덕점",
                    address: "제주시 조천읍 조함해안로 510",
                    map: "https://map.naver.com/p/search/계절식탁%20함덕점",
                    tip: "位於回程路上的咸德海邊。推薦鮑魚粥或海鮮拉麵。<br>💡 周邊：吃完飯可到樓下的咸德海水浴場散步看夜海。"
                },
                {
                    time: "20:00",
                    title: "Olive Young",
                    korean: "올리브영 제주함덕점",
                    address: "제주시 조천읍 조함해안로 526",
                    map: "https://map.naver.com/p/search/올리브영%20제주함덕점",
                    tip: "就在「季節餐桌」隔壁條街上，很方便。"
                },
                {
                    time: "21:00",
                    title: "返回飯店",
                    korean: "-",
                    address: "-",
                    map: "https://map.naver.com/p/search/씨스테이호텔",
                    tip: "從咸德開回涯月 Sea Stay Hotel 約需 50 分鐘，晚上開車請注意安全。"
                }
            ],
            day3: [
                {
                    time: "11:00",
                    title: "West 海濱早午餐 (West Mel)",
                    korean: "웨스트멜",
                    address: "제주시 애월읍 애월해안로 32",
                    map: "https://map.naver.com/p/search/웨스트멜",
                    tip: "離您飯店僅 3 分鐘車程，舒芙蕾鬆餅很有名。"
                },
                {
                    time: "13:00",
                    title: "981 Park (滑坡車)",
                    korean: "9.81파크 제주",
                    address: "제주시 애월읍 천덕로 880-24",
                    map: "https://map.naver.com/p/search/9.81파크",
                    tip: "就在飯店後方的山坡上，車程僅 15 分鐘。<br>💡 必備：**一定要穿包鞋** (禁拖鞋/涼鞋)。務必下載「9.81 Park App」接收賽車影片。"
                },
                {
                    time: "15:30",
                    title: "Mikkang Changgo",
                    korean: "미깡창고",
                    address: "제주시 애월읍 중산간서로 6710-1",
                    map: "https://map.naver.com/p/search/미깡창고",
                    tip: "橘子倉庫改建的網美店。<br>💡 必點：布朗起司可頌鬆餅 (브라운 치즈 크로플)、芝麻拿鐵 (돌담)。"
                },
                {
                    time: "17:00",
                    title: "新羅免稅店",
                    korean: "신라면세점 제주점",
                    address: "제주시 노연로 69",
                    map: "https://map.naver.com/p/search/신라면세점%20제주점",
                    tip: "進入濟州市區（蓮洞商圈）。<br>💡 提醒：**務必攜帶護照** 與 **回程航班資訊**。"
                },
                {
                    time: "19:00",
                    title: "晚餐 & 宵夜",
                    korean: "교촌치킨 (橋村) / BHC 치킨",
                    address: "蓮洞商圈 (外帶)",
                    map: "https://map.naver.com/p/search/제주%20연동%20교촌치킨",
                    tip: "蓮洞商圈非常熱鬧。晚餐後可外帶「橋村炸雞 (Kyochon)」或「BHC 炸雞」回飯店當宵夜。"
                }
            ],
            day4: [
                {
                    time: "11:00",
                    title: "午餐：Galchigwan 涯月店",
                    korean: "갈치관 애월점",
                    address: "제주시 애월읍 애월해안로 686",
                    map: "https://map.naver.com/p/search/갈치관%20애월점",
                    tip: "飯店退房後，沿著海岸路開 4 分鐘即達。<br>💡 特色：有無敵海景，主打「整條去骨白帶魚」，拌飯吃非常美味。"
                },
                {
                    time: "13:00",
                    title: "Haejigae Cafe",
                    korean: "해지개",
                    address: "제주시 애월읍 애월북서길 52",
                    map: "https://map.naver.com/p/search/해지개",
                    tip: "韓屋造型的海景咖啡廳，離飯店僅 2 分鐘車程。<br>💡 必點：黑色起司麵包、橘子蛋糕。<br>💡 注意：**開進去的路非常窄**，會車困難，建議停在大馬路停車場再走進去。"
                },
                {
                    time: "14:30",
                    title: "樂天免稅店",
                    korean: "롯데면세점 제주점",
                    address: "제주시 도령로 83",
                    map: "https://map.naver.com/p/search/롯데면세점%20제주점",
                    tip: "最後補貨時間，位於市區，離機場很近。"
                },
                {
                    time: "16:30",
                    title: "還車",
                    korean: "原租車公司車庫",
                    address: "濟州機場附近 (請依業者指引)",
                    map: "https://map.naver.com/p/search/제주국제공항",
                    tip: "濟州市區下午 17:00 後易塞車，請務必準時或提早還車。定位先設定為機場，請依照您的租車公司指示前往。"
                },
                {
                    time: "17:30",
                    title: "晚餐：Ojik Jeju (機場總店)",
                    korean: "오직흑돼지 제주공항본점",
                    address: "제주시 서해안로 264",
                    map: "https://map.naver.com/p/search/오직흑돼지%20제주공항본점",
                    tip: "位於機場旁的龍潭海岸道路上，方便吃完直達機場。<br>💡 特色：只有單點，肉質優秀，是完美的收尾餐。"
                },
                {
                    time: "19:00",
                    title: "前往機場",
                    korean: "제주국제공항 (CJU)",
                    address: "제주시 공항로 2",
                    map: "https://map.naver.com/p/search/제주국제공항",
                    tip: "準備登機，滿載而歸！"
                }
            ]
        };

        function createItineraryCard(item) {
            const hasMap = item.map;
            const mapButton = hasMap
                ? `<a href="${item.map}" target="_blank" rel="noopener noreferrer" class="inline-block bg-green-500 text-white font-bold py-2 px-3 rounded-lg hover:bg-green-600 transition-colors text-sm">🗺️ Naver Map</a>`
                : '';

            return `
                <div class="itinerary-card">
                    <div class="p-5">
                        <div class="flex justify-between items-start">
                            <div>
                                <div class="text-xs font-semibold text-orange-600 bg-orange-100 inline-block px-3 py-1 rounded-full">${item.time}</div>
                                <h3 class="text-xl font-bold text-gray-900 mt-2">${item.title}</h3>
                            </div>
                            ${hasMap ? '' : '<span class="text-3xl ml-4">✈️</span>'}
                        </div>
                        <div class="mt-3 text-gray-600 text-sm">
                            <p>${item.korean}</p>
                            <p class="font-mono">${item.address}</p>
                        </div>
                    </div>
                    <div class="bg-gray-50 px-5 py-3 border-t border-gray-100">
                        <div class="flex justify-between items-center">
                            <h4 class="font-semibold text-orange-700 text-sm flex items-center">
                                <span class="text-xl mr-1">💡</span> 在地人建議
                            </h4>
                            ${mapButton}
                        </div>
                        <div class="mt-3 pt-3 border-t border-gray-200">
                            <p class="text-gray-700 text-sm">${item.tip}</p>
                        </div>
                    </div>
                </div>
            `;
        }

        document.addEventListener('DOMContentLoaded', () => {
            const day1Content = document.getElementById('day1-content');
            const day2Content = document.getElementById('day2-content');
            const day3Content = document.getElementById('day3-content');
            const day4Content = document.getElementById('day4-content');

            itineraryData.day1.forEach(item => day1Content.innerHTML += createItineraryCard(item));
            itineraryData.day2.forEach(item => day2Content.innerHTML += createItineraryCard(item));
            itineraryData.day3.forEach(item => day3Content.innerHTML += createItineraryCard(item));
            itineraryData.day4.forEach(item => day4Content.innerHTML += createItineraryCard(item));

            /* appContent event listener removed */

            // --- New Navigation Logic ---
            const navSelect = document.getElementById('navigation-select');
            const allSections = document.querySelectorAll('main > section');

            navSelect.addEventListener('change', (e) => {
                const value = e.target.value;

                if (value === 'all') {
                    // Show all sections
                    allSections.forEach(section => {
                        section.style.display = 'block';
                    });
                    // Scroll to top
                    window.scrollTo({ top: 0, behavior: 'smooth' });
                } else {
                    // Hide all sections
                    allSections.forEach(section => {
                        section.style.display = 'none';
                    });
                    // Show the selected one
                    const targetSection = document.querySelector(value);
                    if (targetSection) {
                        targetSection.style.display = 'block';
                        // Scroll to the top of that section
                        targetSection.scrollIntoView({ behavior: 'smooth' });
                    }
                }
            });

            // --- Old Navigation Logic Removed ---

        });
    </script>
</body>
</html>
