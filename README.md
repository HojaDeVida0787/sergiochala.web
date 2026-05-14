<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sergio Alejandro Tapiero Chala</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #ff0000;
            --dark: #ff0000;
            --light: #f8fafc;
            --text-main: #334155;
            --accent: #334155;
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: #f1f5f9;
            color: var(--text-main);
            line-height: 1.6;
            padding-bottom: 40px;
        }

        /* Contenedor Principal */
        .app-container {
            max-width: 500px;
            margin: 0 auto;
            background: white;
            min-height: 100vh;
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
        }

        
        .container {
            max-width: 850px;
            margin: 0 auto;
            background: var(--card-bg);
            padding: 40px;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }   

       /* Cabecera Centrada */
        header {
            text-align: center;
            border-bottom: 3px solid var(--accent-color);
            padding-bottom: 30px;
            margin-bottom: 30px;
        }

        .profile-photo {
            width: 300px;
            height: 300px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid var(--accent-color);
            margin-bottom: 15px;
            box-shadow: 0 8px 40px #1a1e24;
           
        }

        .header-text h1 { margin: 2px 0; color: var(--accent-color); font-size: 2.5em; }
        
        

        .profile-img {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            border: 4px solid var(--accent);
            margin-bottom: 15px;
            object-fit: cover;
            background: #eee;
        }

        h1 { font-size: 1.5rem; margin-bottom: 5px; }
        .tagline { font-weight: 300; opacity: 0.9; font-size: 0.9rem; }

        /* Secciones */
        section { padding: 25px 20px; border-bottom: 1px solid #f1f5f9; }
        h2 { 
            color: var(--primary); 
            font-size: 1.1rem; 
            margin-bottom: 15px; 
            display: flex; 
            align-items: center;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        /* Experiencia */
        .card {
            background: var(--light);
            padding: 15px;
            border-radius: 12px;
            margin-bottom: 15px;
            border-left: 4px solid var(--accent);
        }
        .card h3 { font-size: 1rem; color: var(--dark); }
        .date { font-size: 0.8rem; color: #64748b; font-weight: 600; }
        .desc { font-size: 0.85rem; margin-top: 8px; }

        /* Chips de Conocimientos */
        .skills-grid { display: flex; flex-wrap: wrap; gap: 8px; }
        .skill-chip {
            background: #e2e8f0;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 500;
        }

        /* Botones de Certificados     */

        .cert-link {
             display: block;
            width: 100%;
            padding: 12px;
            background: white;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
            margin-bottom: 10px;
            text-decoration: none;
            color: var(--dark);
            font-size: 0.9rem;
            transition: 0.3s;
            box-shadow: 0 9px 20px #64748b;
            
        }
        .cert-link:active { background: #f1f5f9; transform: scale(0.98); }

         /* Botón de WhatsApp Flotante */
        .btn-whatsapp {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: var(--whatsapp-color);
            background-color: #22c55e;
            color: rgb(255, 255, 255);
            padding: 15px 25px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            box-shadow: 0 4px 15px rgb(21, 255, 0);
            display: flex;
            align-items: center;
            gap: 10px;
            z-index: 1000;
}


        /* Contacto Flotante */
        .fab {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: #22c55e;
            color: white;
            width: 56px;
            height: 56px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 4px 12px #4f46e5;
            text-decoration: none;
            font-weight: bold;
        }


         
            
      
        .btn-whatsapp:hover { transform: scale(1.1); }



         /* Pie de página / Copyright */
        footer {
            text-align: center;
            margin-top: 40px;
            font-size: 0.8em;
            color: #7f8c8d;
            border-top: 1px solid #eee;
            padding-top: 20px;
        }

        /* Animaciones */
        .fade-in {
            animation: fadeIn 0.6s ease-in;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>


     <!-- Botón de WhatsApp -->
    <a href="https://wa.me/573189882787" class="btn-whatsapp" target="_blank">
        <span>WhatsApp</span>
    </a>
    

 <div class="container">
        <header>
            <img src="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/699116233_989437980648237_9201268186456313724_n.jpg?stp=c0.63.944.944a_dst-jpg_s565x565_tt6&_nc_cat=104&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeF20nckf-W9D3ZFO7cEU1xSlECitdgceRmUQKK12Bx5GWvzlgUUxyauRT7-iPD92RZ-aTX-rvfv8ZiXQ66KkWHV&_nc_ohc=qY7a5IYYVpkQ7kNvwHYigno&_nc_oc=Adq7tu2nUG_KDT2COPTg4pOWBEkpBziTfgzlkEL1I2aeyiumO_Wizxcm_bfnwvmjyiM&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=9pUcB9nEIoLEQG6ew28qGQ&_nc_ss=7e2a8&oh=00_Af4Mk7115JuLtd5Te55tnEe20oOrb9pQ2N13O3oZ4KSZdw&oe=6A09DF6A" alt="Foto de Sergio Chala" class="profile-photo">
            
            <div class="header-text">
                <h1>SERGIO CHALA</h1>
                <p><strong>NUIP 1.006.506.890</strong></p>
                <p><strong>BACHILLER - Desarrollador Web & Estratega de Marketing Digital</strong></p>
                <div class="contact-info">
                    
                    <span>📞 +57 318 988 2787</span>
                    <span>✉️ sergiochala250@gmail.com</span>
                    <span>📍 Neiva, Huila</span>
                </div>
            </div>
        </header>

    <section class="fade-in">
        <h2>Sobre Mí</h2>
        <p class="desc">Persona social, positiva y comprometida. Con gran facilidad de aprendizaje y sin limitaciones para enfrentar nuevos retos profesionales.</p>
    </section>

    <section>
        <h2>Experiencia</h2>
        
        <div class="card">
            <h3>Auxiliar Eléctrico - Smartool Company</h3>
            <span class="date">Enero 2026 – Abril 2026</span>
            <p class="desc">Apoyo en excavaciones para acometidas, instalaciones eléctricas y transporte de materiales.</p>
            <section id="certificados"><a href="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/696378892_122097731517318735_7224973262598116403_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=833d8c&_nc_ohc=mIAB6YRv838Q7kNvwFSm5qX&_nc_oc=Adphk6iEQAajuqw8BH7oSV9oVhV08kSk1yxVi3BZhc5nzR81v_9dU2ZxlvIe3gcyedQ&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=bjAWydcGNr6-t5bCqjcUHg&_nc_ss=7e2a8&oh=00_Af4A48EoN9dyc0TInA7gXVO4jbA5k3cWSloT3taIPCpI0g&oe=6A0A60E2" class="cert-link" onclick="alert('Abriendo certificado: Smartool Company')">📄 Certificado Smartool</a></section>
            
        </div>

  
        <div class="card">
            <h3>Auxiliar Eléctrico - Smartool Company</h3>
            <span class="date">Septiembre 2025 – Diciembre 2025</span>
            <p class="desc">Apoyo en excavaciones para acometidas, instalaciones eléctricas y transporte de materiales.</p>
            <section id="certificados"><a href="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/696900937_122097732015318735_2368577302475113626_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=833d8c&_nc_ohc=VcB1Cd8Ek94Q7kNvwH0IdY0&_nc_oc=AdrrVbludgORyGJZ-99l1hIo7koKDcqLdPhVOfgH0Pq0VeJB-6izgNNqNKv6_ts-LaE&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=kgoVwbJH07H7fnzaTbICyg&_nc_ss=7e2a8&oh=00_Af7o5RXjP2RpWACw_3lhPCIA743VBXxfPYfl7U8AZvkFkg&oe=6A0A754A" class="cert-link" onclick="alert('Abriendo certificado: Smartool Company')">📄 Certificado Smartool</a></section>
        </div>

        <div class="card">
            <h3>Brigadista Brigrada - Nases</h3>
            <span class="date">Enero 2025  – Febrero 2025</span>
            <p class="desc">Apoyo en ventas tienda a tienda, Region Huila</p>
            <section id="certificados"><a href="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/697244849_122097734115318735_4491043880404710420_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=833d8c&_nc_ohc=zOamvPdYMacQ7kNvwE7edjZ&_nc_oc=AdqfOODm8DANg2NXEU7_Ml7yQ_XiBHrKsAvQb-fMpzAA3bRq7hEYNqe34gPsZZvzCXo&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=K2Xk6HTOMuUVKKMGh6HPnQ&_nc_ss=7e2a8&oh=00_Af6QwYkRU3S3L0_SL1Q12EoJ4ZWp1nyWm8BS6jCtwx8OwQ&oe=6A0A549C" class="cert-link" onclick="alert('Abriendo certificado: Nases')">📄 Certificado Nases</a></section>

        </div>

        <div class="card">
            <h3>Asesor Comercial - Hogarama</h3>
            <span class="date">Abril 2024 – Diciembre 2024</span>
            <p class="desc">Asesorar a clientes, identificar oportunidades de venta y mantener relaciones sólidas para aumentar las ventas y fidelizar clientes.</p>
            <section id="certificados"><a href="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/695838073_122097734283318735_9053260773741159703_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=833d8c&_nc_ohc=TcFeyq-LMuAQ7kNvwGb2kyT&_nc_oc=AdombfC2hh3x_IKajZXCnLIAc99xoO9KYEzxolXvk5I2RT_iUelJ1_hXvoKiTY9p6Ic&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=yYvxzq4RG67SxrPuhs2-9A&_nc_ss=7e2a8&oh=00_Af4sw0vr8_4bct5geLKE8DCKddzGIgxEqqjvVirdZjh1uw&oe=6A0A54FB" class="cert-link" onclick="alert('Abriendo certificado: Hogarama')">📄 Certificado Hogarama</a></section>

        </div>

        <div class="card">
            <h3>Asesor Comercial - Corálpa</h3>
            <span class="date">Noviembre 2023 – Febrero 2024</span>
            <p class="desc">Asesorar a clientes, identificar oportunidades de venta y mantener relaciones sólidas para aumentar las ventas y fidelizar clientes.</p>
            <section id="certificados"><a href="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/696269624_122097734451318735_2635281416765457152_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=833d8c&_nc_ohc=lNfckOebgEAQ7kNvwFe_Vva&_nc_oc=Adp-PoPm2pctA2WPeaXaBF0sxyARyLTsuiRIaNlnxpJ7sPql2IKw2bUg-Kfcgw0s5L0&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=vBmlec95AhmRmqrMUZfQTw&_nc_ss=7e2a8&oh=00_Af5vx9QwuV5ZuTrjsiXt7za9guKmjJUt-LBBqlCmLdLruQ&oe=6A0A74B8" class="cert-link" onclick="alert('Abriendo certificado: Corálpa')">📄 Certificado Corálpa</a></section>

        </div>
    </section>

    <section>
        <h2>Informática & Herramientas</h2>
        <div class="skills-grid">
            <span class="skill-chip">Maeketing-Facebook-Instagram</span>
            <span class="skill-chip">Microsoft Excel</span>
            <span class="skill-chip">PowerPoint</span>
            <span class="skill-chip">Visual Studio Code</span>
            <span class="skill-chip">Html, Css, JavaScript</span>
            <span class="skill-chip">Marketing Digital</span>
        </div>
    </section>

    <section>
        <h2>Idiomas</h2>
        <p><strong>Español:</strong> Nativo</p>
        <p><strong>Inglés:</strong> Básico</p>
    </section>

    <section id="certificados">
        
        <h2>Certificados de estudios</h2>
        <a href="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/696927605_122097734883318735_3441227986145222739_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=833d8c&_nc_ohc=GTDh_NktZhAQ7kNvwEEYGMw&_nc_oc=AdrHwY7bicXlO48JEkz6npgnhcuWBMnq5ZXwalc3GHhVnplU--X379TgvD3TKcctS70&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=i_oxsMyqtbRfi6uSRkAARQ&_nc_ss=7e2a8&oh=00_Af4t7vF3NjzC8YGYQNz-EmboY76BUMtK8cFSgw3D4TZZsQ&oe=6A0A5414" class="cert-link" onclick="alert('Abriendo certificado: Bachiller Académico')">🎓 Título: Bachiller Académico</a>
        <a href="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/699064497_122097735567318735_4144715802551633318_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=833d8c&_nc_ohc=ArCpyBmA6iEQ7kNvwGIPuzg&_nc_oc=Adp_QknWYb3tAO4jjMnN5_GmEXbp7Yqc0-k-sz2Ky8kCUCLJfFo-LPm6oBmnSUGnZWE&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=1f6M77tF5shFUaYBHLlaZA&_nc_ss=7e2a8&oh=00_Af5hvsiA6iwibTba9LJVqtW0sC3ks8Y2oyBOz2TT-6WeoA&oe=6A0A8836" class="cert-link" onclick="alert('Abriendo certificado: Costrucción básica')">🎓 Otros: Costrucción básica</a>
        <a href="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/699430489_122097735681318735_6393652398998279660_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=833d8c&_nc_ohc=lw13vMXIJdIQ7kNvwEhwFZd&_nc_oc=Ado6cR3ZeY_SeK6UiIBSLPucGaZ2poj6wEqyOHSG4Yv7W36xGoaVDATCcF1QognuBDA&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=Q57ot0lL9p2Y4Q9jWNNhDQ&_nc_ss=7e2a8&oh=00_Af4CEalD0vfHZb11oT0aCkb0YjbZejrHVHhtcjP_qg2Skg&oe=6A0A8265" class="cert-link" onclick="alert('Abriendo certificado: Mantenimiento de motocicletas de propulcion electrica')">🎓 Otros: Mantenimiento de motocicletas de propulcion electrica</a>
        <a href="https://scontent.fnva2-1.fna.fbcdn.net/v/t39.30808-6/697062656_122097736035318735_2548291598145745523_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=833d8c&_nc_ohc=Uc7iXQZ7E5oQ7kNvwFVd58o&_nc_oc=AdovGChA8LXZRs9nnS42aerl8C6XnpVCOgOg1R0lHjvH21UXDivS5nl1aIgtLX5ZwpU&_nc_zt=23&_nc_ht=scontent.fnva2-1.fna&_nc_gid=3fnyd3f82nugPpROyJJpdQ&_nc_ss=7e2a8&oh=00_Af46y8MK1GB0sbWXBz4rgdGggXHRyNkvxY50CEeDJDfWUg&oe=6A0A66BE" class="cert-link" onclick="alert('Abriendo certificado: Mantenimiento preventivo de motocicletas y motocarros')">🎓 Otros: Mantenimiento preventivo de motocicletas y motocarros</a>

    </section>

    <section>
        <h2>Otros Datos</h2>
        <p class="desc">✅ Licencia de conducir A2<br>
        ✅ Vehículo propio<br>
        ✅ Disponibilidad para viajar</p>
    </section>

           <footer>
            &copy; 2024 Sergio Chala. Todos los derechos reservados. <br>
            Generado como Hoja de Vida Profesional.
        </footer>

</div>



<script>
    // Optimización: Efecto de scroll suave y revelación de elementos
    document.addEventListener('DOMContentLoaded', () => {
        const cards = document.querySelectorAll('.card');
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if(entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateX(0)';
                }
            });
        }, { threshold: 0.1 });

        cards.forEach(card => {
            card.style.opacity = '0';
            card.style.transform = 'translateX(-20px)';
            card.style.transition = 'all 0.5s ease-out';
            observer.observe(card);
        });
    });
</script>

</body>
</html>
