<template>
    <div class="header">Philippe's Personal Website</div>

<div class="container">
    <div class="tile" onclick="showContent('about')">About Me</div>
    <div class="tile" onclick="showContent('education')">Education and Achievements</div>
    <div class="tile" onclick="showContent('course')">Course</div>
    <div class="tile" onclick="showContent('experience')">IT Experience</div>
    <div class="tile" onclick="showContent('hobbies')">Hobbies and Interests</div>
    <div class="tile" onclick="showContent('goals')">Goals in Life</div>
    <div class="tile" onclick="showContent('gallery')">Picture Gallery</div>
    <div class="tile" onclick="showContent('links')">Links to Socials</div>
</div>

<div id="about" class="content hidden">
    <h1>About Me</h1>
    <p>Hello! My name is Philippe, I am an aspiring IT student passionate about technology and improving myself.</p>
</div>

<div id="education" class="content hidden">
    <h2>Education and Achievements</h2>
    <ul>
        <li>With High Honors (Malate Catholic School, 2019-2020)</li>
        <li>With Honors (Asia Pacific College, 2023-2024)</li>
    </ul>
</div>

<div id="course" class="content hidden">
    <h2>Course</h2>
    <p>Bachelor of Science in Information Technology Specializing in Mobile and Internet Technology</p>
</div>

<div id="experience" class="content hidden">
    <h2>IT Experience</h2>
    <table>
        <tr>
            <th>Project</th>
            <th>Position</th>
        </tr>
        <tr>
            <td>Tutor Booking App</td>
            <td>UI Designer</td>
        </tr>
        <tr>
            <td>Gamified Course: APC Dungeon</td>
            <td>Head Animator</td>
        </tr>
        <tr>
            <td>Facility Booking System: Rambook</td>
            <td>Head Developer</td>
        </tr>
    </table>
</div>

<div id="hobbies" class="content hidden">
    <h2>Hobbies and Interests</h2>
    <ul>
        <li>Basketball</li>
        <li>Gaming</li>
        <li>Music</li>
        <li>Watching Movies</li>
    </ul>
</div>

<div id="goals" class="content hidden">
    <h2>Goals in Life</h2>
    <p>To be successful in life and give back to my family.</p>
</div>

<div id="gallery" class="content hidden">
    <h2>Picture Gallery</h2>
    <img src="https://scontent.xx.fbcdn.net/v/t1.15752-9/463004261_2023136481489815_4583702698394093898_n.jpg?stp=dst-jpg_s526x395&_nc_cat=103&ccb=1-7&_nc_sid=0024fc&_nc_eui2=AeHETe-I62mx5WuCf1hFSRcd9BIG9SjhkzT0Egb1KOGTNMnaFebwDWHGeu7WYAJPLoLCO_-jkujqK-et6lCDfUmN&_nc_ohc=7Io_GcGx-CkQ7kNvgGCffgS&_nc_ad=z-m&_nc_cid=0&_nc_zt=23&_nc_ht=scontent.xx&oh=03_Q7cD1QGBr9g5ydjjaPCj61xfZgg24AeP-1FcKPHbpRJGnzjKLQ&oe=676F9068" alt="Music">
    <img src="https://scontent.xx.fbcdn.net/v/t1.15752-9/462545799_568958942525309_5011812986289502423_n.jpg?stp=dst-jpg_p480x480&_nc_cat=102&ccb=1-7&_nc_sid=0024fc&_nc_eui2=AeHpVopIRhmZx2J61g_r9gOjd5066H0FuHF3nTrofQW4censVjHKaCzwuNN4Uwk8SJL-xtQIsXuCB6xb5IIP8NgQ&_nc_ohc=x1C5yQDJk0sQ7kNvgHCDmKP&_nc_ad=z-m&_nc_cid=0&_nc_zt=23&_nc_ht=scontent.xx&oh=03_Q7cD1QHcGQP22BsremGYdw7kDxHiCyCtpT9ht4X5LTuaxss1-g&oe=676F94D6" alt="Bonding with friends">
</div>

<div id="links" class="content hidden">
    <h2>Links to Socials</h2>
    <ul>
        <li><a href="https://github.com/pilepsgithvb">Github Account</a></li>
        <li><a href="https://www.linkedin.com/in/philippe-gerong-67705a24a">LinkedIn Profile</a></li>
    </ul>
</div>
</template>

<script>
        function showContent(id) {
            const contents = document.querySelectorAll('.content');
            contents.forEach(content => content.classList.add('hidden'));
            document.getElementById(id).classList.remove('hidden');
        }
    </script>

<style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            background-color: #f8f8f8;
        }

        .header {
            background: linear-gradient(to bottom, #e52d27, #b31217);
            color: white;
            padding: 20px;
            margin-bottom: 20px;
            font-size: 24px;
            font-weight: bold;
            text-transform: uppercase;
            border: 4px solid white;
            display: inline-block;
            border-radius: 8px;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            max-width: 1200px;
            margin: auto;
        }

        .tile {
            background-color: #e0e0e0;
            width: 150px;
            height: 100px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            border: 2px solid black;
            border-radius: 8px;
            cursor: pointer;
            font-weight: bold;
            text-transform: uppercase;
        }

        .tile:hover {
            background-color: #d1d1d1;
        }

        .hidden {
            display: none;
        }

        .content {
            margin-top: 20px;
            padding: 20px;
            background-color: white;
            border: 2px solid #ccc;
            border-radius: 8px;
            max-width: 800px;
            margin: 20px auto;
            text-align: left;
        }

        .content img {
            max-width: 100px;
            margin: 10px;
        }

        .content table {
            width: 100%;
            border-collapse: collapse;
        }

        .content table, .content th, .content td {
            border: 1px solid black;
        }

        .content th, .content td {
            padding: 8px;
            text-align: center;
        }

        a {
            text-decoration: none;
            color: blue;
        }
 
</style>