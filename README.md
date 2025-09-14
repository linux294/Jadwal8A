
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jadwal Kelas 8A</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            padding: 10px;
            font-size: 14px;
        }
        
        .container {
            max-width: 100%;
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            overflow: hidden;
        }
        
        .header {
            background-color: #2196F3;
            color: white;
            padding: 15px;
            text-align: center;
        }
        
        .header h1 {
            font-size: 18px;
            margin-bottom: 5px;
        }
        
        .header h2 {
            font-size: 14px;
            font-weight: normal;
        }
        
        .day-tabs {
            display: flex;
            background-color: #f5f5f5;
            overflow-x: auto;
        }
        
        .day-tab {
            flex: 1;
            padding: 12px 8px;
            text-align: center;
            background-color: #ddd;
            border: none;
            font-size: 12px;
            cursor: pointer;
            white-space: nowrap;
            min-width: 60px;
        }
        
        .day-tab.active {
            background-color: #4CAF50;
            color: white;
        }
        
        .schedule-content {
            padding: 15px;
        }
        
        .day-schedule {
            display: none;
        }
        
        .day-schedule.active {
            display: block;
        }
        
        .time-block {
            background: white;
            border: 1px solid #ddd;
            border-radius: 6px;
            margin-bottom: 8px;
            padding: 10px;
        }
        
        .time-header {
            background-color: #FF9800;
            color: white;
            padding: 6px 8px;
            border-radius: 4px;
            font-weight: bold;
            font-size: 12px;
            margin-bottom: 8px;
        }
        
        .subject-name {
            font-weight: bold;
            font-size: 14px;
            color: #333;
            margin-bottom: 3px;
        }
        
        .teacher-name {
            font-size: 11px;
            color: #666;
        }
        
        .break-block {
            background-color: #FFC107;
            color: black;
            text-align: center;
            padding: 10px;
            border-radius: 6px;
            margin-bottom: 8px;
            font-weight: bold;
        }
        
        .footer {
            background-color: #37474F;
            color: white;
            padding: 12px;
            text-align: center;
        }
        
        .footer div {
            margin-bottom: 8px;
        }
        
        .footer h4 {
            font-size: 12px;
            margin-bottom: 3px;
        }
        
        .footer p {
            font-size: 10px;
            margin: 1px 0;
        }
        
        .current-time {
            background-color: #2196F3;
            color: white;
            padding: 8px;
            text-align: center;
            font-size: 12px;
            margin-bottom: 10px;
            border-radius: 4px;
        }
    </style>
</head>
<body>
    <div class="container">
        <header class="header">
            <h1>JADWAL KELAS 8A</h1>
            <h2>SMPN 1 TAMBUN SELATAN</h2>
        </header>
        
        <div class="current-time" id="currentTime"></div>
        
        <div class="day-tabs">
            <button class="day-tab active" onclick="showDay('senin')">SENIN</button>
            <button class="day-tab" onclick="showDay('selasa')">SELASA</button>
            <button class="day-tab" onclick="showDay('rabu')">RABU</button>
            <button class="day-tab" onclick="showDay('kamis')">KAMIS</button>
            <button class="day-tab" onclick="showDay('jumat')">JUMAT</button>
        </div>
        
        <div class="schedule-content">
            <!-- SENIN -->
            <div id="senin" class="day-schedule active">
                <div class="break-block">06.30-07.15 | Kokurikuler</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 1 | 07.15-07.55</div>
                    <div class="subject-name">PA BP</div>
                    <div class="teacher-name">Aan Andawiyah, S.Ag.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 2 | 07.55-08.35</div>
                    <div class="subject-name">PA BP</div>
                    <div class="teacher-name">Aan Andawiyah, S.Ag.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 3 | 08.35-09.15</div>
                    <div class="subject-name">IPS</div>
                    <div class="teacher-name">Purnia, S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 4 | 09.15-09.55</div>
                    <div class="subject-name">IPS</div>
                    <div class="teacher-name">Purnia, S.Pd.</div>
                </div>
                
                <div class="break-block">09.55-10.25 | ISTIRAHAT I</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 5 | 10.25-11.05</div>
                    <div class="subject-name">B. Sunda</div>
                    <div class="teacher-name">Winwin W., S.S.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 6 | 11.05-11.45</div>
                    <div class="subject-name">B. Indonesia</div>
                    <div class="teacher-name">Adah, S.Pd.</div>
                </div>
                
                <div class="break-block">11.45-12.35 | ISHOMA + MBG</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 7 | 12.35-13.15</div>
                    <div class="subject-name">B. Indonesia</div>
                    <div class="teacher-name">Adah, S.Pd.</div>
                </div>
            </div>
            
            <!-- SELASA -->
            <div id="selasa" class="day-schedule">
                <div class="break-block">06.30-07.15 | Kokurikuler</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 1 | 07.15-07.55</div>
                    <div class="subject-name">Baca Tulis Qur'an</div>
                    <div class="teacher-name">Aan Andawiyah, S.Ag.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 2 | 07.55-08.35</div>
                    <div class="subject-name">B. Inggris</div>
                    <div class="teacher-name">Anani Mulyani, S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 3 | 08.35-09.15</div>
                    <div class="subject-name">IPA</div>
                    <div class="teacher-name">Anjar Bayu K., S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 4 | 09.15-09.55</div>
                    <div class="subject-name">IPA</div>
                    <div class="teacher-name">Anjar Bayu K., S.Pd.</div>
                </div>
                
                <div class="break-block">09.55-10.25 | ISTIRAHAT I</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 5 | 10.25-11.05</div>
                    <div class="subject-name">Informatika</div>
                    <div class="teacher-name">Mujianto, S.Kom.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 6 | 11.05-11.45</div>
                    <div class="subject-name">Informatika</div>
                    <div class="teacher-name">Mujianto, S.Kom.</div>
                </div>
                
                <div class="break-block">11.45-12.35 | ISHOMA + MBG</div>
            </div>
            
            <!-- RABU -->
            <div id="rabu" class="day-schedule">
                <div class="break-block">06.30-07.15 | Kokurikuler</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 1 | 07.15-07.55</div>
                    <div class="subject-name">B. Indonesia</div>
                    <div class="teacher-name">Adah, S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 2 | 07.55-08.35</div>
                    <div class="subject-name">Matematika</div>
                    <div class="teacher-name">Ida Susanti, S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 3 | 08.35-09.15</div>
                    <div class="subject-name">Matematika</div>
                    <div class="teacher-name">Ida Susanti, S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 4 | 09.15-09.55</div>
                    <div class="subject-name">Pend. Pancasila</div>
                    <div class="teacher-name">Marlita Sutiawati, SH.</div>
                </div>
                
                <div class="break-block">09.55-10.25 | ISTIRAHAT I</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 5 | 10.25-11.05</div>
                    <div class="subject-name">Pend. Pancasila</div>
                    <div class="teacher-name">Marlita Sutiawati, SH.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 6 | 11.05-11.45</div>
                    <div class="subject-name">Prakarya</div>
                    <div class="teacher-name">Surandini Wahyu, S.Pd.</div>
                </div>
                
                <div class="break-block">11.45-12.35 | ISHOMA + MBG</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 7 | 12.35-13.15</div>
                    <div class="subject-name">Prakarya</div>
                    <div class="teacher-name">Surandini Wahyu, S.Pd.</div>
                </div>
            </div>
            
            <!-- KAMIS -->
            <div id="kamis" class="day-schedule">
                <div class="break-block">06.30-07.15 | Kokurikuler</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 1 | 07.15-07.55</div>
                    <div class="subject-name">PJOK</div>
                    <div class="teacher-name">Hasbi Hadi R., S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 2 | 07.55-08.35</div>
                    <div class="subject-name">PJOK</div>
                    <div class="teacher-name">Hasbi Hadi R., S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 3 | 08.35-09.15</div>
                    <div class="subject-name">BK</div>
                    <div class="teacher-name">Dra. Rita Puspita</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 4 | 09.15-09.55</div>
                    <div class="subject-name">IPS</div>
                    <div class="teacher-name">Purnia, S.Pd.</div>
                </div>
                
                <div class="break-block">09.55-10.25 | ISTIRAHAT I</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 5 | 10.25-11.05</div>
                    <div class="subject-name">Matematika</div>
                    <div class="teacher-name">Ida Susanti, S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 6 | 11.05-11.45</div>
                    <div class="subject-name">Matematika</div>
                    <div class="teacher-name">Ida Susanti, S.Pd.</div>
                </div>
                
                <div class="break-block">11.45-12.35 | ISHOMA + MBG</div>
            </div>
            
            <!-- JUMAT -->
            <div id="jumat" class="day-schedule">
                <div class="break-block">06.30-07.15 | Kokurikuler</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 1 | 07.15-07.55</div>
                    <div class="subject-name">B. Indonesia</div>
                    <div class="teacher-name">Adah, S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 2 | 07.55-08.35</div>
                    <div class="subject-name">B. Indonesia</div>
                    <div class="teacher-name">Adah, S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 3 | 08.35-09.15</div>
                    <div class="subject-name">IPA</div>
                    <div class="teacher-name">Anjar Bayu K., S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 4 | 09.15-09.55</div>
                    <div class="subject-name">IPA</div>
                    <div class="teacher-name">Anjar Bayu K., S.Pd.</div>
                </div>
                
                <div class="break-block">09.55-10.25 | ISTIRAHAT I</div>
                
                <div class="time-block">
                    <div class="time-header">JAM 5 | 10.25-11.05</div>
                    <div class="subject-name">B. Inggris</div>
                    <div class="teacher-name">Anani Mulyani, S.Pd.</div>
                </div>
                
                <div class="time-block">
                    <div class="time-header">JAM 6 | 11.05-11.45</div>
                    <div class="subject-name">B. Inggris</div>
                    <div class="teacher-name">Anani Mulyani, S.Pd.</div>
                </div>
                
                <div class="break-block">11.45-12.35 | ISHOMA + MBG</div>
            </div>
        </div>
        
        <footer class="footer">
            <div>
                <h4>Kepala Sekolah</h4>
                <p>Dr. Hj. Annisa, S.Pd. M.Pd.</p>
            </div>
            <div>
                <h4>Wali Kelas 8A</h4>
                <p>Adang, S.Kom.</p>
            </div>
            <div style="margin-top: 15px; padding-top: 10px; border-top: 1px solid #555;">
                <h4>Dibuat oleh</h4>
                <p><strong>Faishal Amir Kahllis</strong></p>
                <p style="font-size: 9px; opacity: 0.7;">Website Developer</p>
            </div>
        </footer>
    </div>

    <script>
        function showDay(day) {
            // Hide all day schedules
            const schedules = document.querySelectorAll('.day-schedule');
            schedules.forEach(schedule => {
                schedule.classList.remove('active');
            });
            
            // Remove active class from all tabs
            const tabs = document.querySelectorAll('.day-tab');
            tabs.forEach(tab => {
                tab.classList.remove('active');
            });
            
            // Show selected day
            document.getElementById(day).classList.add('active');
            
            // Add active class to clicked tab
            event.target.classList.add('active');
        }
        
        function updateTime() {
            const now = new Date();
            const days = ['Minggu', 'Senin', 'Selasa', 'Rabu', 'Kamis', 'Jumat', 'Sabtu'];
            const months = ['Jan', 'Feb', 'Mar', 'Apr', 'Mei', 'Jun', 'Jul', 'Ags', 'Sep', 'Okt', 'Nov', 'Des'];
            
            const dayName = days[now.getDay()];
            const date = now.getDate();
            const month = months[now.getMonth()];
            const hours = now.getHours().toString().padStart(2, '0');
            const minutes = now.getMinutes().toString().padStart(2, '0');
            
            document.getElementById('currentTime').textContent = 
                `${dayName}, ${date} ${month} - ${hours}:${minutes}`;
        }
        
        // Update time every minute
        setInterval(updateTime, 60000);
        updateTime();
        
        // Auto-select current day
        const today = new Date().getDay();
        const dayNames = ['minggu', 'senin', 'selasa', 'rabu', 'kamis', 'jumat', 'sabtu'];
        if (today >= 1 && today <= 5) {
            showDay(dayNames[today]);
        }
    </script>
</body>
</html>
