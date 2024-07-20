<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Political System of India</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
        }

        header {
            background: #333;
            color: #fff;
            padding: 1rem 0;
            text-align: center;
        }

        nav ul {
            list-style: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin: 0 1rem;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
        }

        main {
            padding: 2rem;
        }

        section {
            margin-bottom: 2rem;
        }

        footer {
            text-align: center;
            padding: 1rem 0;
            background: #333;
            color: #fff;
        }

        .leader-img {
            width: 400px;
            height: auto;
            display: block;
            margin: 1rem 0;
            transition: transform 0.3s ease-in-out;
        }

        .leader-img:hover {
            transform: scale(1.1);
        }

        .graphics {
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 2rem 0;
        }

        .graphics img {
            width: 150px;
            height: auto;
            margin: 0 1rem;
            opacity: 0.8;
            transition: opacity 0.3s ease-in-out;
        }

        .graphics img:hover {
            opacity: 1;
        }

        h2 {
            color: #4CAF50;
            transition: color 0.5s ease-in-out, transform 0.5s ease-in-out;
        }

        h2:hover {
            color: #FF5722;
            transform: translateX(10px);
        }

        #structure h2 {
            color: #2196F3;
        }

        #structure h2:hover {
            color: #FFC107;
        }

        #parties h2 {
            color: #9C27B0;
        }

        #parties h2:hover {
            color: #E91E63;
        }

        #media h2 {
            color: #00BCD4;
        }

        #media h2:hover {
            color: #FF9800;
        }

        #elections h2 {
            color: #FF5722;
        }

        #elections h2:hover {
            color: #4CAF50;
        }

        #judiciary h2 {
            color: #673AB7;
        }

        #judiciary h2:hover {
            color: #CDDC39;
        }

        #issues h2 {
            color: #FFC107;
        }

        #issues h2:hover {
            color: #2196F3;
        }

        #corruption h2 {
            color: #E91E63;
        }

        #corruption h2:hover {
            color: #00BCD4;
        }
    </style>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const parties = [
                { 
                    name: "Bharatiya Janata Party", 
                    leader: "Narendra Modi", 
                    img: "https://assets.telegraphindia.com/telegraph/0b8014a0-68e9-4c3c-8a5f-d4df4a03f1af.jpg" 
                },
                { 
                    name: "Indian National Congress", 
                    leader: "Rahul Gandhi", 
                    img: "https://tse1.mm.bing.net/th?id=OIP.wbTjLJunG9SS6HgfDVzc8wHaEK&pid=Api&P=0&h=180" 
                },
                { 
                    name: "Aam Aadmi Party", 
                    leader: "Arvind Kejriwal", 
                    img: "https://akm-img-a-in.tosshub.com/sites/dailyo/fb_feed_images/story_image/201901/arvind-1820_010119012632.jpg" 
                }
            ];

            const partyList = document.getElementById("partyList");

            parties.forEach(function(party) {
                const listItem = document.createElement("li");
                listItem.innerHTML = <strong>${party.name}</strong> - Leader: ${party.leader}<br><img src="${party.img}" alt="${party.leader}" class="leader-img">;
                partyList.appendChild(listItem);
            });

            function showPartyLeader(partyName) {
                const party = parties.find(p => p.name === partyName);
                if (party) {
                    alert(The leader of ${party.name} is ${party.leader});
                } else {
                    alert("Party not found.");
                }
            }

            // Example of conditional statement
            if (parties.length > 3) {
                console.log("There are more than 3 major parties in India.");
            } else {
                console.log("There are 3 or fewer major parties in India.");
            }
        });
    </script>
</head>
<body>
    <header>
        <h1>Political System of India</h1>
        <nav>
            <ul>
                <li><a href="#introduction">Introduction</a></li>
                <li><a href="#structure">Structure</a></li>
                <li><a href="#parties">Major Parties</a></li>
                <li><a href="#media">Media</a></li>
                <li><a href="#elections">Elections</a></li>
                <li><a href="#judiciary">Judiciary</a></li>
                <li><a href="#issues">Issues</a></li>
                <li><a href="#corruption">Corruption</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="introduction">
            <h2>Introduction</h2>
            <p>India is a federal parliamentary democratic republic, where the President is the head of state, and the Prime Minister is the head of government. The political system has evolved over centuries, influenced by various historical and cultural factors.</p>
        </section>
        <section id="structure">
            <h2>Structure</h2>
            <p>The political system of India is structured into three main branches: Executive, Legislative, and Judiciary. The Executive branch is headed by the President, the Legislative branch is a bicameral Parliament, and the Judiciary is an independent body.</p>
            <img src="https://gkindiatoday.com/wp-content/uploads/2018/07/Indian-political-parties.jpg" alt="Political Structure of India" class="leader-img">
        </section>
        <section id="parties">
            <h2>Major Parties</h2>
            <p>Here are the major political parties in India:</p>
            <ul id="partyList"></ul>
        </section>
        <section id="media">
            <h2>Media</h2>
            <p>The media plays a crucial role in Indian politics by providing information and acting as a watchdog. It includes newspapers, television, radio, and digital platforms.</p>
        </section>
        <section id="elections">
            <h2>Elections</h2>
            <p>Elections in India are conducted by the Election Commission of India. They are held at various levels including national, state, and local levels. The General Elections are held every five years to elect members of the Lok Sabha.</p>
        </section>
        <section id="judiciary">
            <h2>Judiciary</h2>
            <p>The Judiciary in India is an independent branch of government that interprets and applies the law. It ensures the constitutionality of laws and resolves disputes. The Supreme Court is the highest judicial authority in India.</p>
        </section>
        <section id="issues">
            <h2>Political Issues</h2>
            <p>India faces several political issues, including regionalism, casteism, and communalism. These issues often influence voting patterns and political alliances, impacting the stability and functionality of governments.</p>
        </section>
        <section id="corruption">
            <h2>Corruption</h2>
            <p>Corruption is a significant issue in Indian politics, affecting various levels of government. Efforts to combat corruption include legislation, anti-corruption bodies, and public awareness campaigns.</p>
        </section>
    </main>
    <div class="graphics">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/41/Flag_of_India.svg/1920px-Flag_of_India.svg.png" alt="Flag of India">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/Emblem_of_India_%28without_motto%29.svg/1200px-Emblem_of_India_%28without_motto%29.svg.png" alt="Emblem of India">
    </div>
    <footer>
        <p>&copy; 2024 Jashandeep and Gurleen</p>
    </footer>
</body>
</html>
