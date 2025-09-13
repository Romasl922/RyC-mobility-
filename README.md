<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Servicio de Transporte Ejecutivo - Romano Sandoval Lizano</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .bg-pattern {
            background-image: url('https://placehold.co/1200x800/2a2a2a/f9f9f9?text=Fondo+de+pantalla');
            background-size: cover;
            background-position: center;
        }
        .glass-bg {
            background: rgba(43, 43, 43, 0.5);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .fade-in-on-load {
            animation: fadeIn 1s ease-in-out;
        }
    </style>
</head>
<body class="bg-gray-900 text-white leading-relaxed">

    <!-- Hero Section -->
    <header class="relative flex items-center justify-center min-h-screen bg-pattern">
        <div class="absolute inset-0 bg-gray-900 bg-opacity-70"></div>
        <div class="relative z-10 text-center p-6 md:p-12 fade-in-on-load">
            <h1 class="text-4xl sm:text-5xl md:text-7xl font-bold mb-4">
                <span class="block">RyC Mobility Solutions</span>
                <span class="block text-xl md:text-3xl font-medium text-gray-400 mt-2">Transporte ejecutivo y transporte aeropuerto</span>
            </h1>
            <p class="text-lg md:text-xl max-w-2xl mx-auto mb-8 text-gray-300">
                Ofrecemos un servicio de transporte privado, seguro y puntual, con la comodidad y exclusividad que usted merece.
            </p>
            <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                <button id="openBookingModal" class="bg-teal-500 hover:bg-teal-600 text-white font-bold py-3 px-8 rounded-full shadow-lg transition duration-300 ease-in-out transform hover:scale-105">
                    Reservar Ahora
                </button>
                <a href="https://wa.me/50664499462" target="_blank" class="bg-green-500 hover:bg-green-600 text-white font-bold py-3 px-8 rounded-full shadow-lg transition duration-300 ease-in-out transform hover:scale-105">
                    Consultar por WhatsApp
                </a>
            </div>
        </div>
    </header>

    <!-- Services Section -->
    <main class="container mx-auto px-4 py-16">
        <section class="mb-16">
            <h2 class="text-4xl font-bold text-center mb-12">Nuestros Servicios</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 md:gap-12">
                <!-- Servicio de Transporte al Aeropuerto -->
                <div class="glass-bg p-8 rounded-3xl shadow-lg transform transition duration-300 hover:scale-105 text-center">
                    <div class="w-full h-56 rounded-2xl overflow-hidden mb-6">
                         <!-- Imagen actualizada con la que proporcionaste -->
                        <img src="uploaded:image.png-c8c041f4-06b6-4315-8d9e-a3e4d7d97e81" alt="Transporte al aeropuerto, tu comodidad y seguridad" class="w-full h-full object-cover">
                    </div>
                    <h3 class="text-2xl font-semibold text-teal-300 mb-3">Transporte al y desde el Aeropuerto</h3>
                    <p class="text-gray-300">
                        Viaje sin preocupaciones. Le garantizamos puntualidad para sus vuelos de salida y una bienvenida personalizada a su llegada.
                    </p>
                </div>

                <!-- Servicio de Transporte Ejecutivo -->
                <div class="glass-bg p-8 rounded-3xl shadow-lg transform transition duration-300 hover:scale-105 text-center">
                    <div class="w-full h-56 rounded-2xl overflow-hidden mb-6">
                        <!-- Imagen actualizada con la que proporcionaste -->
                        <img src="uploaded:image.png-d7a24948-59bd-480c-b38d-9e9756f4c7b5" alt="Servicio de transporte ejecutivo de lujo" class="w-full h-full object-cover">
                    </div>
                    <h3 class="text-2xl font-semibold text-teal-300 mb-3">Transporte Ejecutivo Privado</h3>
                    <p class="text-gray-300">
                        Ideal para reuniones de negocios, eventos especiales o traslados discretos. Nuestro servicio le brinda privacidad y confort en todo momento.
                    </p>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section class="text-center md:text-left mb-16">
            <div class="glass-bg p-8 md:p-12 rounded-3xl shadow-lg flex flex-col md:flex-row items-center gap-8">
                <div class="w-40 h-40 md:w-48 md:h-48 rounded-full overflow-hidden shrink-0">
                    <!-- Imagen de perfil actualizada con la que proporcionaste -->
                    <img src="uploaded:image.png-c06f63ec-9ac7-4c58-b1b3-d4545502baec" alt="Foto de Romano Sandoval Lizano" class="w-full h-full object-cover">
                </div>
                <div>
                    <h2 class="text-3xl font-bold mb-4">Sobre Romano Sandoval Lizano</h2>
                    <p class="text-gray-300">
                        Mi objetivo es ofrecer un servicio de transporte que vaya más allá de simplemente trasladar personas. Me enfoco en la seguridad, la puntualidad y una experiencia de cliente superior. Confíe en mí para sus viajes más importantes.
                    </p>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section class="text-center">
            <h2 class="text-4xl font-bold mb-8">Contáctame</h2>
            <div class="text-gray-300">
                <p class="mb-2">Teléfono: <a href="tel:64499462" class="text-teal-400 hover:underline">6449-9462</a></p>
                <p>Correo: <a href="mailto:romasl87@gmail.com" class="text-teal-400 hover:underline">romasl87@gmail.com</a></p>
            </div>
        </section>
    </main>

    <!-- Booking Modal -->
    <div id="bookingModal" class="fixed inset-0 bg-gray-900 bg-opacity-80 flex items-center justify-center p-4 z-50 hidden">
        <div class="glass-bg p-8 rounded-3xl w-full max-w-2xl shadow-xl transform scale-95 transition-transform duration-300 ease-in-out">
            <div class="flex justify-between items-center mb-6">
                <h3 class="text-2xl font-bold">Realizar Reserva</h3>
                <button id="closeBookingModal" class="text-gray-400 hover:text-white transition duration-300">&times;</button>
            </div>
            <form id="bookingForm" class="grid grid-cols-1 md:grid-cols-2 gap-6 relative z-10">
                <div class="col-span-1">
                    <label for="name" class="block text-gray-300 font-medium mb-1">Nombre</label>
                    <input type="text" id="name" name="name" required class="w-full p-3 bg-gray-800 rounded-lg border border-gray-700 focus:outline-none focus:ring-2 focus:ring-teal-500">
                </div>
                <div class="col-span-1">
                    <label for="phone" class="block text-gray-300 font-medium mb-1">Número de Teléfono</label>
                    <input type="tel" id="phone" name="phone" required class="w-full p-3 bg-gray-800 rounded-lg border border-gray-700 focus:outline-none focus:ring-2 focus:ring-teal-500">
                </div>
                <div class="col-span-2">
                    <label for="serviceType" class="block text-gray-300 font-medium mb-1">Tipo de Servicio</label>
                    <select id="serviceType" name="serviceType" required class="w-full p-3 bg-gray-800 rounded-lg border border-gray-700 focus:outline-none focus:ring-2 focus:ring-teal-500">
                        <option value="Transporte Ejecutivo">Transporte Ejecutivo</option>
                        <option value="Transporte Aeropuerto">Transporte al Aeropuerto</option>
                    </select>
                </div>
                <div class="col-span-1">
                    <label for="date" class="block text-gray-300 font-medium mb-1">Fecha</label>
                    <input type="date" id="date" name="date" required class="w-full p-3 bg-gray-800 rounded-lg border border-gray-700 focus:outline-none focus:ring-2 focus:ring-teal-500">
                </div>
                <div class="col-span-1">
                    <label for="time" class="block text-gray-300 font-medium mb-1">Hora</label>
                    <input type="time" id="time" name="time" required class="w-full p-3 bg-gray-800 rounded-lg border border-gray-700 focus:outline-none focus:ring-2 focus:ring-teal-500">
                </div>
                <div class="col-span-2">
                    <label for="pickupLocation" class="block text-gray-300 font-medium mb-1">Lugar de inicio de viaje</label>
                    <input type="text" id="pickupLocation" name="pickupLocation" required class="w-full p-3 bg-gray-800 rounded-lg border border-gray-700 focus:outline-none focus:ring-2 focus:ring-teal-500">
                </div>
                <div class="col-span-2">
                    <label for="destination" class="block text-gray-300 font-medium mb-1">Lugar de Destino</label>
                    <input type="text" id="destination" name="destination" required class="w-full p-3 bg-gray-800 rounded-lg border border-gray-700 focus:outline-none focus:ring-2 focus:ring-teal-500">
                </div>
                <div class="col-span-2">
                    <button type="submit" class="w-full bg-teal-500 hover:bg-teal-600 text-white font-bold py-3 px-6 rounded-full transition duration-300 transform hover:scale-105">
                        Enviar Reserva por Correo
                    </button>
                </div>
            </form>
        </div>
    </div>

    <!-- JavaScript para la funcionalidad de la página -->
    <script>
        const bookingModal = document.getElementById('bookingModal');
        const openBookingBtn = document.getElementById('openBookingModal');
        const closeBookingBtn = document.getElementById('closeBookingModal');
        const bookingForm = document.getElementById('bookingForm');
        
        // Abrir el modal
        openBookingBtn.addEventListener('click', () => {
            bookingModal.classList.remove('hidden');
        });

        // Cerrar el modal
        closeBookingBtn.addEventListener('click', () => {
            bookingModal.classList.add('hidden');
        });

        // Cerrar el modal al hacer clic fuera del formulario
        bookingModal.addEventListener('click', (e) => {
            if (e.target === bookingModal) {
                bookingModal.classList.add('hidden');
            }
        });

        // Manejar el envío del formulario
        bookingForm.addEventListener('submit', (e) => {
            e.preventDefault();

            const name = document.getElementById('name').value;
            const phone = document.getElementById('phone').value;
            const serviceType = document.getElementById('serviceType').value;
            const date = document.getElementById('date').value;
            const time = document.getElementById('time').value;
            const pickupLocation = document.getElementById('pickupLocation').value;
            const destination = document.getElementById('destination').value;

            const subject = `Nueva Reserva de Transporte de ${name}`;
            const body = `Hola Romano,\n\nRecibiste una nueva reserva de transporte.\n\n` +
                         `Nombre: ${name}\n` +
                         `Teléfono: ${phone}\n` +
                         `Servicio: ${serviceType}\n` +
                         `Fecha: ${date}\n` +
                         `Hora: ${time}\n` +
                         `Lugar de inicio de viaje: ${pickupLocation}\n` +
                         `Destino: ${destination}\n\n` +
                         `Por favor, confirma esta reserva lo antes posible.`;

            // Encodifica el asunto y el cuerpo del correo para la URL
            const mailtoLink = `mailto:romasl87@gmail.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;

            // Abre el cliente de correo del usuario
            window.location.href = mailtoLink;

            // Opcional: cierra el modal después de que el cliente de correo se abre.
            // Es mejor mantener el modal abierto para que el usuario sepa que la acción se ha iniciado.
            // bookingModal.classList.add('hidden');
        });
    </script>
</body>
</html>

