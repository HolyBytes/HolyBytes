<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ADE PRATAMA - GitHub Profile</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/js/all.min.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background-color: #0d1117;
            color: #c9d1d9;
            line-height: 1.6;
        }
        
        .container {
            max-width: 900px;
            margin: 30px auto;
            padding: 20px;
        }
        
        .header {
            display: flex;
            align-items: center;
            margin-bottom: 30px;
            border-bottom: 1px solid #30363d;
            padding-bottom: 20px;
        }
        
        .profile-img {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid #58a6ff;
            background: linear-gradient(135deg, #6e8efb, #a777e3);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 50px;
            color: white;
        }
        
        .profile-info {
            margin-left: 20px;
        }
        
        .profile-info h1 {
            font-size: 28px;
            margin-bottom: 5px;
            color: #e6edf3;
        }
        
        .profile-info p {
            color: #8b949e;
            margin-bottom: 10px;
        }
        
        .card {
            background-color: #161b22;
            border-radius: 6px;
            padding: 20px;
            margin-bottom: 20px;
            border: 1px solid #30363d;
        }
        
        .bio-card {
            background: linear-gradient(135deg, #161b22, #1f2937);
            border: 1px solid #30363d;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        
        .bio-card h2 {
            color: #58a6ff;
            margin-bottom: 15px;
            border-bottom: 1px solid #30363d;
            padding-bottom: 10px;
        }
        
        .bio-content {
            display: flex;
            flex-wrap: wrap;
        }
        
        .bio-item {
            width: 50%;
            margin-bottom: 10px;
        }
        
        .bio-item strong {
            color: #8b949e;
        }
        
        .story {
            background: linear-gradient(135deg, #1f2937, #171c24);
            border-radius: 10px;
            padding: 20px;
            margin-top: 20px;
            border-left: 4px solid #58a6ff;
        }
        
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 20px;
        }
        
        .skill {
            background: #21262d;
            border-radius: 20px;
            padding: 8px 16px;
            font-size: 14px;
            color: #e6edf3;
            display: flex;
            align-items: center;
            gap: 8px;
            transition: all 0.3s ease;
        }
        
        .skill:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .skill-icon {
            width: 18px;
            height: 18px;
        }
        
        .stats {
            display: flex;
            gap: 20px;
            margin-top: 30px;
        }
        
        .stat-card {
            flex: 1;
            background: #161b22;
            border-radius: 10px;
            padding: 15px;
            text-align: center;
            border: 1px solid #30363d;
            transition: all 0.3s ease;
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .stat-value {
            font-size: 24px;
            font-weight: 600;
            color: #58a6ff;
        }
        
        .stat-label {
            font-size: 12px;
            color: #8b949e;
        }
        
        .github-calendar {
            background: #161b22;
            border-radius: 10px;
            padding: 20px;
            margin-top: 20px;
            border: 1px solid #30363d;
        }
        
        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            grid-template-rows: repeat(7, 1fr);
            gap: 3px;
            margin-top: 15px;
        }
        
        .calendar-day {
            width: 100%;
            padding-top: 100%;
            position: relative;
            border-radius: 2px;
        }
        
        footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #30363d;
            color: #8b949e;
            font-size: 14px;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
            justify-content: center;
        }
        
        .social-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: #21262d;
            color: #c9d1d9;
            transition: all 0.3s ease;
        }
        
        .social-btn:hover {
            transform: translateY(-3px);
            background: #30363d;
            color: #58a6ff;
        }
        
        .html { background: linear-gradient(135deg, #e34c26, #f06529); }
        .css { background: linear-gradient(135deg, #264de4, #2965f1); }
        .bootstrap { background: linear-gradient(135deg, #563d7c, #7952b3); }
        .java { background: linear-gradient(135deg, #5382a1, #f89820); }
        .javascript { background: linear-gradient(135deg, #f0db4f, #f7df1e); }
        .nodejs { background: linear-gradient(135deg, #3c873a, #68a063); }
        .php { background: linear-gradient(135deg, #777bb3, #8892bf); }
        .mysql { background: linear-gradient(135deg, #00618a, #0082c6); }
        
        .repo-card {
            padding: 15px;
            background: #21262d;
            border-radius: 6px;
            margin-bottom: 15px;
            border: 1px solid #30363d;
            transition: all 0.3s ease;
        }
        
        .repo-card:hover {
            transform: translateY(-3px);
            border-color: #58a6ff;
        }
        
        .repo-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 10px;
        }
        
        .repo-name {
            color: #58a6ff;
            font-weight: 600;
        }
        
        .repo-stats {
            display: flex;
            gap: 15px;
        }
        
        .repo-stat {
            display: flex;
            align-items: center;
            gap: 5px;
            font-size: 12px;
            color: #8b949e;
        }
        
        .repo-desc {
            font-size: 14px;
            color: #c9d1d9;
            margin-bottom: 10px;
        }
        
        .repo-langs {
            display: flex;
            gap: 10px;
        }
        
        .repo-lang {
            display: flex;
            align-items: center;
            gap: 5px;
            font-size: 12px;
            color: #8b949e;
        }
        
        .lang-color {
            width: 10px;
            height: 10px;
            border-radius: 50%;
        }
        
        .pinned-repos {
            margin-top: 30px;
        }

        @media (max-width: 768px) {
            .header {
                flex-direction: column;
                text-align: center;
            }
            
            .profile-info {
                margin-left: 0;
                margin-top: 15px;
            }
            
            .bio-item {
                width: 100%;
            }
            
            .stats {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="profile-img">AP</div>
            <div class="profile-info">
                <h1>ADE PRATAMA</h1>
                <p>@adepratama | Calon Web Developer & Game Developer</p>
                <p><i class="fas fa-map-marker-alt"></i> SMK Negeri 1 Pulau Rakyat, Indonesia</p>
                <div class="social-links">
                    <a href="#" class="social-btn"><i class="fab fa-github"></i></a>
                    <a href="#" class="social-btn"><i class="fab fa-linkedin"></i></a>
                    <a href="#" class="social-btn"><i class="fab fa-instagram"></i></a>
                    <a href="#" class="social-btn"><i class="fab fa-twitter"></i></a>
                </div>
            </div>
        </div>
        
        <div class="bio-card">
            <h2>Tentang Saya</h2>
            <div class="bio-content">
                <div class="bio-item"><strong>Nama:</strong> ADE PRATAMA</div>
                <div class="bio-item"><strong>Kelas:</strong> 12 TKJ3</div>
                <div class="bio-item"><strong>Sekolah:</strong> SMK Negeri 1 Pulau Rakyat</div>
                <div class="bio-item"><strong>Cita-cita:</strong> Web Developer & Game Developer</div>
            </div>
            
            <div class="story">
                <p>Aku mulai suka sama dunia pemrograman waktu di MTs, awalnya cuma iseng main game Free Fire tapi lama-lama penasaran gimana sih cara bikin game sebagus itu? Dari situlah aku mulai belajar otodidak dengan alat sederhana yang aku punya. Meskipun awalnya susah banget, tapi aku nggak nyerah dan terus belajar sampai sekarang. Mimpi aku bisa jadi web developer dan game developer profesional! 🚀</p>
            </div>
            
            <h2 style="margin-top: 20px;">Skills & Tech Stack</h2>
            <div class="skills">
                <div class="skill html">
                    <i class="fab fa-html5"></i> HTML
                </div>
                <div class="skill css">
                    <i class="fab fa-css3-alt"></i> CSS
                </div>
                <div class="skill bootstrap">
                    <i class="fab fa-bootstrap"></i> Bootstrap
                </div>
                <div class="skill java">
                    <i class="fab fa-java"></i> Java
                </div>
                <div class="skill javascript">
                    <i class="fab fa-js"></i> JavaScript
                </div>
                <div class="skill nodejs">
                    <i class="fab fa-node-js"></i> Node.js
                </div>
                <div class="skill php">
                    <i class="fab fa-php"></i> PHP
                </div>
                <div class="skill mysql">
                    <i class="fas fa-database"></i> MySQL
                </div>
            </div>
        </div>
        
        <div class="stats">
            <div class="stat-card">
                <div class="stat-value">12</div>
                <div class="stat-label">Repositories</div>
            </div>
            <div class="stat-card">
                <div class="stat-value">85</div>
                <div class="stat-label">Kontribusi Tahun Ini</div>
            </div>
            <div class="stat-card">
                <div class="stat-value">24</div>
                <div class="stat-label">Followers</div>
            </div>
            <div class="stat-card">
                <div class="stat-value">37</div>
                <div class="stat-label">Following</div>
            </div>
        </div>
        
        <div class="github-calendar">
            <h3>Aktivitas GitHub</h3>
            <div class="calendar-grid">
                <!-- Simulasi calendar activity dengan warna acak -->
                <script>
                    document.addEventListener('DOMContentLoaded', () => {
                        const calendarGrid = document.querySelector('.calendar-grid');
                        const colors = ['#0e4429', '#006d32', '#26a641', '#39d353'];
                        
                        for (let i = 0; i < 49; i++) {
                            const day = document.createElement('div');
                            day.className = 'calendar-day';
                            
                            // Generate random contribution level
                            const rand = Math.random();
                            if (rand > 0.6) {
                                const colorIndex = Math.floor(Math.random() * colors.length);
                                day.style.backgroundColor = colors[colorIndex];
                            } else {
                                day.style.backgroundColor = '#161b22';
                            }
                            
                            calendarGrid.appendChild(day);
                        }
                    });
                </script>
            </div>
        </div>
        
        <div class="pinned-repos">
            <h3>Project Teratas</h3>
            
            <div class="repo-card">
                <div class="repo-header">
                    <span class="repo-name">game-adventure-2D</span>
                    <div class="repo-stats">
                        <span class="repo-stat"><i class="far fa-star"></i> 15</span>
                        <span class="repo-stat"><i class="fas fa-code-branch"></i> 5</span>
                    </div>
                </div>
                <p class="repo-desc">Game petualangan 2D sederhana yang dibuat dengan Java. Project ini adalah game platformer pertama saya.</p>
                <div class="repo-langs">
                    <span class="repo-lang">
                        <span class="lang-color" style="background-color: #b07219;"></span>
                        Java
                    </span>
                </div>
            </div>
            
            <div class="repo-card">
                <div class="repo-header">
                    <span class="repo-name">website-portfolio</span>
                    <div class="repo-stats">
                        <span class="repo-stat"><i class="far fa-star"></i> 8</span>
                        <span class="repo-stat"><i class="fas fa-code-branch"></i> 2</span>
                    </div>
                </div>
                <p class="repo-desc">Website portfolio responsive yang menampilkan project dan skill saya dalam dunia web development.</p>
                <div class="repo-langs">
                    <span class="repo-lang">
                        <span class="lang-color" style="background-color: #e34c26;"></span>
                        HTML
                    </span>
                    <span class="repo-lang">
                        <span class="lang-color" style="background-color: #563d7c;"></span>
                        CSS
                    </span>
                    <span class="repo-lang">
                        <span class="lang-color" style="background-color: #f1e05a;"></span>
                        JavaScript
                    </span>
                </div>
            </div>
            
            <div class="repo-card">
                <div class="repo-header">
                    <span class="repo-name">sistem-manajemen-perpustakaan</span>
                    <div class="repo-stats">
                        <span class="repo-stat"><i class="far fa-star"></i> 12</span>
                        <span class="repo-stat"><i class="fas fa-code-branch"></i> 4</span>
                    </div>
                </div>
                <p class="repo-desc">Aplikasi sistem manajemen perpustakaan berbasis web dengan fitur pinjam, kembali, dan katalog buku.</p>
                <div class="repo-langs">
                    <span class="repo-lang">
                        <span class="lang-color" style="background-color: #4F5D95;"></span>
                        PHP
                    </span>
                    <span class="repo-lang">
                        <span class="lang-color" style="background-color: #00758F;"></span>
                        MySQL
                    </span>
                    <span class="repo-lang">
                        <span class="lang-color" style="background-color: #563d7c;"></span>
                        Bootstrap
                    </span>
                </div>
            </div>
        </div>
        
        <footer>
            <p>Dibuat dengan ❤️ oleh ADE PRATAMA &copy; 2025</p>
            <p>Jangan lupa follow untuk update project terbaru!</p>
        </footer>
    </div>
</body>
</html>
