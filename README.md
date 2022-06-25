/* 
Public Kirka.io CSS #2 by NizzQ#9235
Please do give credit if you decided to recolor :)

-=Install Instructions for Browser=-
    1. Install "Stylus" extension
	2. Create a new style
	3. Paste the source code into it or you can just C&P "@import url(https://nizzq.github.io/NizzQ2.css)" for updates
	4. Enable it

-=Install Instructions for Client=-
	1. https://nizzq.github.io/NizzQ2.css
 */
/* Fonts */
@font-face {
    font-family: gamefont;
    src: url("https://raw.githubusercontent.com/MOF1/krunker_css/main/css/fonts/Steradian-Bold.otf");
}

* {
    font-family: gamefont;
}

/* Hide Logo */
.interface .logo {
    display: none;
}

/*	Ad Removal */
#ad-bottom,
#ad-left {
    visibility: hidden;
}

/* Animation */
@-webkit-keyframes glow {
    from {
        text-shadow: 0 0 5px #fff, 0 0 5px #ae50e4, 0 0 5px #ae50e4, 0 0 5px #ae50e4, 0 0 6px #ae50e4, 0 0 7px #ae50e4, 0 0 8px #ae50e4;
    }
}

@-webkit-keyframes animate{
    to {transform:translateY(30%);}
}

@keyframes rainbow{
		100%,0%{
			color: rgb(255,0,0);
		}
		8%{
			color: rgb(255,127,0);
		}
		16%{
			color: rgb(255,255,0);
		}
		25%{
			color: rgb(127,255,0);
		}
		33%{
			color: rgb(0,255,0);
		}
		41%{
			color: rgb(0,255,127);
		}
		50%{
			color: rgb(0,255,255);
		}
		58%{
			color: rgb(0,127,255);
		}
		66%{
			color: rgb(0,0,255);
		}
		75%{
			color: rgb(127,0,255);
		}
		83%{
			color: rgb(255,0,255);
		}
		91%{
			color: rgb(255,0,127);
		}
}

/* Background */
.pattern-bg,
.bg-radial {
    display: none;
}

.interface .background{
    background: url(https://media.discordapp.net/attachments/944281177030815764/990335085016383498/903390_1.png?width=1165&height=656) repeat !important;
    height: 300%;
    background-position: 0px 0px;
    -webkit-animation: animate 10s linear infinite!important;
}

.end-modal {
    background: url(https://media.discordapp.net/attachments/944281177030815764/990335085016383498/903390_1.png?width=1165&height=656) repeat !important;
}

/* Loading Scene*/
.loading-scene .progress {
    background: -webkit-gradient(linear, left top, right top, from(#84a1ff), to(#39ffd4)) !important;
    background: linear-gradient(to right, #84a1ff, #39ffd4) !important;
}

.loading-scene .name .label {
    -webkit-animation: glow 2s ease-in-out infinite alternate;
    -moz-animation: glow 2s ease-in-out infinite alternate;
    animation: glow 2s ease-in-out infinite alternate;
}

.loading-scene .players .level {
    color: white;
}

/* Join URL Button (For client only) */
.join-using-link {
    background: rgba(55, 55, 55, .61) !important;
    border-radius: 0 !important;
    border: 4px solid #ffffff1c !important;
}

.join-using-link:active {
    background: #39ffd4bf!important;
}

#clientJoinButton {
	background: rgba(55, 55, 55, .61) !important;
    border-radius: 0 !important;
    border: 4px solid #ffffff1c !important;
}

#clientJoinButton:active {
    background: #39ffd4bf!important;
}

/* Stream */
.live-streams {
    background: rgba(55, 55, 55, .61);
    backdrop-filter: blur(5px);
    position: fixed;
    left: 95px;
    top: 80px;
    width: 300px !important;
    height: 1200px;
    border-left: 4px solid #ffffff1c;
    -webkit-transition: 0.8s;
    transition: 0.8s;
}

.live-streams:before {
    content: url(https://media.discordapp.net/attachments/523517791886770188/947364113770758194/pngfind.com-chevron-png-95287.png?width=30&height=30);
    position: fixed;
    right: 320px;
    top: 15px;
    transition: 0.2s;
}

.live-streams:hover:before {
    opacity: 0;
}

.live-streams:after {
    content: "CSS by NizzQ#9235";
    position: fixed;
    top: 505px;
    right: 115px;
}

.live-streams:hover {
    left: -115px;
}

.live-streams .head {
    display: none;
}

.live-streams .list {
    width: 180px;
    padding: 0 9px;
    overflow: visible;
}

/* Login/Signup*/
.auth-form {
    margin-left: 0 !important;
    background: rgba(55, 55, 55, .61) !important;
    backdrop-filter: blur(5px);
    border: none !important;
    border-left: none !important;
    border-right: none !important;
    box-shadow: none !important;
    border-bottom: 5px solid #ffffff1c !important;
    border-radius: 0 !important;
    width: 2500px;
    height: 112px;
}

.auth-form .btns button {
    margin-top: 20px;
    transform: none !important;
    padding: 0px;
}


.auth-user .loading {
    background: rgba(55, 55, 55, .61);
	backdrop-filter: blur(5px);
	border: none;
	border-bottom: 5px solid #ffffff1c !important;
	border-radius: 0;
	width: 2500px;
    height: 112px;
}

.auth-user .loader-container {
	margin-right: 95% !important;
}

.button[data-v-02c36fca] {
    -webkit-text-stroke: 0px !important;
}

.auth-form .btns button:hover {
    background-color: transparent !important;
    box-shadow: none !important;
}

.auth-form button,
.auth-form button .border-top,
.auth-form button .border-bottom{
    background: transparent !important;
    box-shadow: none !important;
}

.auth-form button .triangle {
    display: none;
}

.auth-form .text {
    font-size: 30px !important;
}

.auth-form button:hover {
    color: #30e7ff;
}

.button[data-v-02c36fca]:after {
    border: none;
}

/* Left Interface*/
.left-interface {
    margin-left: 109px;
}

.left-interface .profile {
    background: rgba(55, 55, 55, .61);
    backdrop-filter: blur(5px);
    width: 2500px;
    border-bottom: 5px solid #ffffff1c;
}

.left-interface .progress-label {
    display: none;
}

.left-interface .progress-lvl {
    margin-bottom: 20px;
}

.left-interface .progress-line {
    background: #4f4e4ead !important;
    height: 17px;
}

.left-interface .progress {
    background: -webkit-gradient(linear, left top, right top, from(#84a1ff), to(#39ffd4)) !important;
    background: linear-gradient(to right, #84a1ff, #39ffd4) !important;
}

.left-interface .level {
    color: white;
}

.left-interface .avatar-info,
.left-interface .user-info,
.left-interface .money {
    background: transparent !important;
    border-top: none !important;
    border-bottom: none !important;
}

.left-interface .avatar-info:hover,
.left-interface .user-info:hover {
    background: transparent;
}

/* Left icons */
.left-icons {
    background: rgba(55, 55, 55, .61);
    backdrop-filter: blur(5px);
    top: 0 !important;
    left: 0 !important;
    width: 112px;
    height: 2000px;
    border-right: 5px solid #ffffff1c;
}

.left-icons .icon-btn {
    background: transparent;
    border-top: none;
    border-bottom: none;
    width: 107px;
    height: 100px;
    margin: 0;
    border-radius: 0;
}

.left-icons .icon-btn:hover {
    border-top: none;
}

.left-icons .icon-btn:hover > .wrapper[data-v-ae524044] {
    transform: none;
}

.left-icons .icon-btn .text-icon,
.left-icons .icon-btn svg {
    display: none;
}

.left-icons .icon-btn svg {
    margin-top: 13px !important;
    transition: 0.3s;
}

.left-icons .icon-btn:nth-child(1) {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946791854823862342/clipart3359599.png?width=676&height=676);
    background-size: 55px !important;
    background-repeat: no-repeat;
    margin-top: 0;
    background-position-x: 1.5rem !important;
    background-position-y: 1rem !important;
    transition: 0.3s;
}

.left-icons .icon-btn:nth-child(1):hover {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946791854823862342/clipart3359599.png?width=676&height=676);
    background-repeat: no-repeat;
    transform: scale(1.2)
}

.left-icons #icon-store {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946792665842843659/Daco_4606909.png);
    background-size: 55px !important;
    background-repeat: no-repeat;
    margin-top: 0;
    background-position-x: 1.5rem !important;
    background-position-y: 1rem !important;
    transition: 0.3s;
}

.left-icons #icon-store:hover {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946792665842843659/Daco_4606909.png);
    background-repeat: no-repeat;
    transform: scale(1.2)
}

.left-icons .icon-btn:nth-child(3) {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946793692327452762/527-5276041_server-png-images-server-icon-free-download-server.png);
    background-size: 55px !important;
    background-repeat: no-repeat;
    margin-top: 0;
    background-position-x: 1.5rem !important;
    background-position-y: 1rem !important;
    transition: 0.3s;
}

.left-icons .icon-btn:nth-child(3):hover {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946793692327452762/527-5276041_server-png-images-server-icon-free-download-server.png);
    background-repeat: no-repeat;
    transform: scale(1.2)
}

.left-icons .icon-btn:nth-child(4) {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946794301529137253/Daco_4390267.png?width=675&height=676);
    background-size: 55px !important;
    background-repeat: no-repeat;
    margin-top: 0;
    background-position-x: 1.5rem !important;
    background-position-y: 1rem !important;
    transition: 0.3s;
}

.left-icons .icon-btn:nth-child(4):hover {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946794301529137253/Daco_4390267.png?width=675&height=676);
    background-repeat: no-repeat;
    transform: scale(1.2)
}

.left-icons .icon-btn[style="--i:5;"] {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946795092310634516/4p200a01ofji3u61huvfc21j8f.png?width=691&height=676);
    background-size: 70px !important;
    background-repeat: no-repeat;
    margin-top: 0;
    background-position-x: 1rem !important;
    background-position-y: 1rem !important;
    transition: 0.3s;
}

.left-icons .icon-btn[style="--i:5;"]:hover {
    background: url(https://media.discordapp.net/attachments/523517791886770188/946795092310634516/4p200a01ofji3u61huvfc21j8f.png?width=691&height=676);
    background-repeat: no-repeat;
    transform: scale(1.2)
}

/* Right Interface */
.soc-group:nth-child(1),
.text-soc {
    display: none !important;
}

.soc-group:nth-child(2) {
    background: url(https://media.discordapp.net/attachments/523517791886770188/947500791365787729/monitor-512.png) !important;
    background-repeat: no-repeat !important;
    background-size: 50px !important;
    background-position-x: 1rem !important;
    background-position-y: 1rem !important;
    border-top: none;
    border-bottom: none;
    position: fixed;
    right: 80px;
    top: 12px;
}

.soc-group:nth-child(2):hover {
    background: url(https://media.discordapp.net/attachments/523517791886770188/947500791365787729/monitor-512.png) !important;
    background-repeat: no-repeat !important;
    background-size: 50px !important;
    background-position-x: 1rem !important;
    background-position-y: 1rem !important;
    transform: scale(1.2);
}

.soc-group:nth-child(2) svg {
    opacity: 0;
}

.right-interface {
    z-index: 999!important;
}

.right-interface .settings {
    background: transparent !important;
    border-bottom: transparent !important;
    border-top: transparent !important;
    margin-top: 30px;
    transition: 0.3s !important;
}

.right-interface .settings:hover {
    transform: scale(1.2)
}

/* Right Icons */
.right-icons .icon-btn {
    background: transparent;
    border-top: none;
    border-bottom: none;
    border-radius: 0;
}


.right-icons .icon-btn:hover {
    border-top: none;
    border-bottom: 3px solid white !important;
}

.right-icons .icon-btn:hover > .wrapper[data-v-ae524044] {
    transform: none;
}

.right-icons .inventory-card {
    background: transparent;
    border-top: none;
    border-bottom: none;
    border-radius: 0;
}

.right-icons .inventory-card:hover {
    background: transparent;
    border-bottom: 3px solid white;
}


/* Container */
.container {
    background: #101216 !important;
    box-shadow: none !important;
    border-radius: 0 !important;
}

.container-card {
    background: #101216 !important;
    box-shadow: none !important;
    border: none !important;
    border-radius: 0 !important;
}

.loader  {
    background: transparent !important;
    border: none !important;
}

.background {
    background: transparent !important;
    border-radius: 0;
}

.tabs {
    background: transparent !important;
    border-bottom: none !important;
    box-shadow: none !important;
    border-right: none !important;
}

.tab {
    background: transparent !important;
    border-right: none !important;
    border-left: none !important;
}

.tab:hover,
.nav:hover {
	color: #39ffd4 !important;
}

.tab.active {
	color: #39ffd4;
	border-bottom: 3px solid #39ffd4;
}

.active-tab {
	color: #39ffd4 !important;
	border-bottom: 3px solid #39ffd4;
}

.nav.active {
	color: #39ffd4;
}

.head-text {
    background: transparent !important;
    box-shadow: none !important;
}

.add-friends,
.top-items {
    background: transparent !important;
}

.limit {
    border-left: none !important;
}

.top-bar,
.close[data-v-747e6ab9],
.home,
.name-page,
.select-mods-cont hr,
.info-icon,
.container button .border-top,
.container button .border-bottom {
    display: none !important;
}

.reset-time,
.info-awards,
.news {
    background: transparent !important;
    box-shadow: none !important;
}

.settings .box {
    background: transparent;
    border: none;
}

.select-mods-cont {
    width: 400px !important;
    height: 587px !important;
    border: none !important;
    border-radius: 0 !important;
    background: #101216 !important;
    overflow: visible;
}

.interface.text-2 > .play > div > .play-content-up > div > div > .select-mods-maps {
    display: grid;
    text-align: left;
    padding: 0 19px;
    width: 100% !important;
    height: 75% !important;
}

.select-regions-cont {
    border: none !important;
    border-radius: 0 !important;
    background: #101216 !important;
    margin-bottom: 40px;
}

.container button {
    background: rgb(68, 68, 68) !important;
    border-radius: 0 !important;
    transform: none !important;
}

.container button .border-top,
.container button .border-bottom {
    display: none;
}

.text {
    transform: none !important;
}

.settings .header,
.vm--container .cont .head {
	color: white !important;
}

.settings .label {
	color: #87898c ;
}

.select-regions-regions .region:nth-child(1) span,
.select-regions-regions .region:nth-child(2) span,
.select-regions-regions .region:nth-child(3) span,
.select-mods-mods .mod:nth-child(1) span,
.select-mods-mods .mod:nth-child(2) span {
	visibility: hidden;
}

.select-regions-regions .region:nth-child(1) span:before,
.select-regions-regions .region:nth-child(2) span:before,
.select-regions-regions .region:nth-child(3) span:before,
.select-mods-mods .mod:nth-child(1) span:before,
.select-mods-mods .mod:nth-child(2) span:before {
	visibility: visible;
}

.select-regions-regions .region:nth-child(1) span:after{
	visibility: visible;
	content: "NA";
	margin-left: -130px;
}

.select-regions-regions .region:nth-child(2) span:after{
	visibility: visible;
	content: "EU";
	margin-left: -60px;
}

.select-regions-regions .region:nth-child(3) span:after{
	visibility: visible;
	content: "SEA";
	margin-left: -32px;
}

.select-mods-mods .mod:nth-child(1) span:after{
	visibility: visible;
	content: "FFA";
	margin-left: -40px;
}

.select-mods-mods .mod:nth-child(2) span:after{
	visibility: visible;
	content: "TDM";
	margin-left: -47px;
}

/* Profile */
.profile .statistics,
.profile .progress,
.profile .k-d,
.card-profile {
    background: transparent !important;
    box-shadow: none !important;
}

.profile .you {
    visibility: hidden;
}

.profile .progress-line {
    background: #4f4e4ead;
}

.profile .progress-level-value,
.stat-name {
    color: white !important;
}

.profile .progress[data-v-5aafd15a] {
    background: -webkit-gradient(linear, left top, right top, from(#84a1ff), to(#39ffd4)) !important;
    background: linear-gradient(to right, #84a1ff, #39ffd4) !important;
}

/*
.heads .clan-tag {
    -webkit-animation: glow 2s ease-in-out infinite alternate;
    -moz-animation: glow 2s ease-in-out infinite alternate;
    animation: glow 2s ease-in-out infinite alternate;
}
*/

.heads .clan-tag {
	animation: rainbow 1.3s linear infinite;
}

.heads .levels {
    display: none;
}

.stat-value {
    color: #87898c !important;
}

.news img {
    border-radius: 0 !important;
}

.news .info {
    background: #101216 !important;
}

.news .info-content {
    background: #101216 !important;
}

.info h1 {
    background: #101216 !important;
}

.changelog-item {
    background: transparent !important;
    border: none !important;
}

/* Inventory */
.tab-bar,
.subject,
.inventory .avatar {
    background: transparent !important;
}

.subjects,
.gun {
    background: transparent !important;
    border: none !important;
}

.inventory .avatar-head {
    display: none;
}

.inventory .bottom {
    background: transparent !important;
    backdrop-filter: blur(2px) !important;
    background-image: linear-gradient(to left, #39ffd400, #39ffd417) !important;
}

/* Play Content */
.play-content .select-region,
.play-content .select-mod {
    background: rgba(55, 55, 55, .61);
    border-radius: 0;
    border: 4px solid #ffffff1c;
}

.play-content .select-region:hover {
    background: rgba(55, 55, 55, .61);
    backdrop-filter: blur(5px);
}

.play-content .select-mod:hover {
    background: rgba(55, 55, 55, .61);
}

#play-btn {
    background: rgba(68, 68, 68, .45) !important;
    width: 310px;
    box-shadow: none !important;
    transform: none !important;
}

#play-btn:hover {
    background: #39ffd4bf !important;
}

#play-btn .border-top,
#play-btn .border-bottom {
    background: none !important;
}

.triangle[data-v-02c36fca] {
    display: none !important;
}

/* Leaderboard */
.leaders .clan-tag {
    -webkit-animation: glow 2s ease-in-out infinite alternate;
    -moz-animation: glow 2s ease-in-out infinite alternate;
    animation: glow 2s ease-in-out infinite alternate;
}

.lvl-leader {
    color: white !important;
}

.list-cont,
.list-champions,
.top-items .items .item,
.bottom-items .item,
.leaderboard-cont .items {
    background: transparent !important;
    box-shadow: none !important;
}

.list-players .top-items {
    box-shadow: none !important;
}

/* Clan */
.clans,
.clans .items .item,
.my-clan .list-container .list .item .item-content {
    background: transparent !important;
}

.my-clan .card-cont,
.my-clan .list-container,
.champions-list {
    background: transparent !important;
    box-shadow: none !important;
}

.my-clan .card-cont .name {
	color: #af51e6;
	-webkit-animation: glow 2s ease-in-out infinite alternate;
    -moz-animation: glow 2s ease-in-out infinite alternate;
    animation: glow 2s ease-in-out infinite alternate;
}

.my-clan .champions-league,
.my-clan .champions-scores,
.my-clan .all-scores-label {
	color: white !important;
}

.my-clan .champions-values,
.my-clan .all-scores-value,
.my-clan .description {
	color: #87898c;
}

/* Market */
.bottom-subj .count {
    background: transparent;
}

/* Esc Interface*/
.esc-interface {
    backdrop-filter: blur(5px);
}

.esc-interface .head-right button,
.esc-interface .head-right button .border-top,
.esc-interface .head-right button .border-bottom {
    background: #101216 !important;
    box-shadow: none;
    border-radius: 0;
}

.esc-interface .head-right button:hover {
    background: #101216 !important;
    border-bottom: 5px solid white;
}

.esc-interface .left-container .player {
    background: transparent;
    background-image: linear-gradient(to left, #39ffd408, #39ffd440) !important;
}

.esc-interface .right-container {
    background: transparent !important;
}

.esc-interface .player .label {
    -webkit-animation: glow 2s ease-in-out infinite alternate;
    -moz-animation: glow 2s ease-in-out infinite alternate;
    animation: glow 2s ease-in-out infinite alternate;
}

.esc-interface .primary {
	color: #39ffd4 !important;
}

.esc-interface .level{
	color: white;
}

.continue {
	background: rgb(68, 68, 68) !important;
	box-shadow: none !important;
}

.continue .border-top,
.continue .border-bottom {
	background: transparent !important;
	box-shadow: none !important;
}

/* HUD */
.mini-map-cont .name,
.info-key-cont,
.list-weapons,
.hp-title,
.mWwn,
.instruction {
    display: none !important;
}

.cont-hp {
    background: transparent !important;
}

.hp {
    margin-right: 20%;
}

.hp-progress {
    background: #8bff9f !important;
}

.desktop-game-interface .state {
    position: fixed;
    width: 500px !important;
    top: 93%;
    left: 37% !important;
}

.cont-endurance {
    margin-left: 1.5%;
    background: transparent !important;
}

.endurance-progress {
	background: -webkit-gradient(linear, left top, right top, from(#84a1ff), to(#39ffd4)) !important;
    background: linear-gradient(to right, #84a1ff, #39ffd4) !important;
}

.weapons-cont {
    position: fixed;
    width: 100px;
    top: 101%;
    left: 5%;
    margin-top: -100px;
    margin-left: 252px;
}

.ammunition {
    display: inline-block;
    position: fixed;
    left: calc(53% + 180px);
}

.kill-death {
    margin-top: 60px;
    margin-left: 2px;
}

.kill-death .kill,
.kill-death .death {
    background: transparent;
    box-shadow: none;
}

.state-cont .timer {
    position: fixed;
    top: 18px;
    background: transparent !important;
    box-shadow: none !important;
    font-size: 50px;
}

/* In Game Leaderboard */
.tab-info {
    background: rgba(55, 55, 55, .61) !important;
	box-shadow: none !important;
	border-radius: 0 !important;
	border: 5px solid #ffffff1c;
}

.tab-info .head {
	display: none;
}

.tab-info .player {
	background: transparent !important;	
}

.tab-info .primary {
	color: white !important;
}

.tab-info .nickname,
.tab-info .player-right {
	color: #87898c;
}

.tab-info .list {
	color: white;
	margin: 0 !important;
}

.tab-info .list .list-value:nth-child(1),
.tab-info .list .list-value:nth-child(2),
.tab-info .list .list-value:nth-child(3) {
	visibility: hidden;
}

.tab-info .list .list-value:nth-child(1):after {
	visibility: visible;
	content: "K";
	margin-left: -29px;
}

.tab-info .list .list-value:nth-child(2):after {
	visibility: visible;
	content: "D";
	margin-left: -28px;
}

.tab-info .list .list-value:nth-child(3):after {
	visibility: visible;
	content: "S";
	margin-left: -5px;
}

.tab-info .player-right svg {
	display: none;
}

.achive-cont {
  	content: url(https://media.discordapp.net/attachments/523517791886770188/956029712470253598/PikPng.com_roblox-head-png_965768.png?width=160&height=160) !important;
  	position: fixed;
  	right: 45%;
}

.kill-bar-item {
	background: rgba(55, 55, 55, .61) !important;
	border: 3px solid red;
}

.kill-bar-item .name {
	color: #8badd6;
}

.kill-bar-item .name-kill {
	color: #f1c876;
}

/* Chat */
.chat {
    margin-bottom: -53px;
    border-radius: 5px;
    -webkit-mask-image: linear-gradient(to bottom, transparent, black, black);
}

.chat .input-wrapper {
    top: 400px !important;
    width: 103%;
    height: 15px;
}

.chat .name {
    color: white;
}

.message{
    color: #87898c !important;
}

.message .lvl {
    color: #39ffd4;
}

/* End Screen */
.end-modal .bottom {
    display: none;
}

.end-modal .progress-line {
    background: #4f4e4ead;
}

.end-modal .progress {
    background: -webkit-gradient(linear, left top, right top, from(#84a1ff), to(#39ffd4)) !important;
    background: linear-gradient(to right, #84a1ff, #39ffd4) !important;
}

.end-modal .team-list-players .card-cont:nth-child(1),
.end-modal .team-list-players .card-cont:nth-child(2),
.end-modal .items {
    background: transparent !important;
    box-shadow: none !important;
}

.end-modal .team-list-players .label {
    background: transparent;
}

.end-modal .label-text,
.end-modal .points,
.end-modal .lvl-leader {
    color: white;
}

.end-modal .chat {
    margin-bottom: -53px;
    border-radius: 5px;
    -webkit-mask-image: linear-gradient(to bottom, transparent, black, black);
}

.end-modal .chat .input-wrapper {
    top: 400px !important;
    width: 103%;
    height: 130px;
}

.end-modal #WMNn {
    width: 310px;
    margin-left: 20px;
}

.end-modal .team-list-players .list .player {
    background: transparent;
}

.end-modal .clan-tag {
    -webkit-animation: glow 2s ease-in-out infinite alternate;
    -moz-animation: glow 2s ease-in-out infinite alternate;
    animation: glow 2s ease-in-out infinite alternate;
}

/* Reward Container */
.progress[data-v-27921169],
.lvl[data-v-27921169],
.progress-helper {
    background: -webkit-gradient(linear, left top, right top, from(#84a1ff), to(#39ffd4)) !important;
    background: linear-gradient(to right, #84a1ff, #39ffd4) !important;
}

.level-head {
    display: none !important;
}

.decor-bg {
	display: none;
}

/* Inputs */
.private-btn > span[data-v-47e1b746] {
	content: url(https://media.discordapp.net/attachments/523517791886770188/953239076457316382/openlock.png);
	position: fixed;
	left: 25px;
	width: 40px;
}

.private-btn > input:checked + span[data-v-47e1b746] {
    content: url(https://media.discordapp.net/attachments/523517791886770188/953239093955948544/lock.png);
}

.custom-checkbox > span[data-v-47e1b746]:before {
    border-radius: 50px;
    background-color: white;
    border: none;
}

.custom-checkbox > input:checked + span[data-v-47e1b746]:before {
    background-color: #2ac144;
}

input {
    background: white !important;
    color: black !important;
    border-radius: 10px !important;
}

.selected {
    background: #292e39;
}

.items {
    background: #292e39 !important;
    box-shadow: none !important;
}

.settings .input {
    background: transparent !important;
    border: none !important;
    box-shadow: none !important;
    color: white !important;
}

.copy button {
	background: rgba(55, 55, 55, .61) !important;
	box-shadow: none !important;
}

.copy .border {
	display: none;
}
