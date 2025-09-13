<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Romano Sandoval Transportes</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            @apply bg-gray-50 text-gray-800;
        }
        /* Custom scroll behavior for sections */
        .section-link {
            cursor: pointer;
        }
        .section-link:hover {
            text-decoration: underline;
        }
        /* Modal backdrop styles */
        .modal-backdrop {
            background-color: rgba(0, 0, 0, 0.5);
        }
        /* Modal content styles */
        .modal-content {
            animation: slide-up 0.3s ease-out;
        }
        @keyframes slide-up {
            from {
                transform: translateY(20px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }
    </style>
</head>
<body>

    <!-- Header / Navbar -->
    <header class="bg-white shadow-md fixed w-full z-10">
        <nav class="container mx-auto px-6 py-4 flex items-center justify-between">
            <a href="#" class="flex items-center space-x-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-indigo-600" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-9v9a1 1 0 01-1 1h-3m-6 0h6m-6 0v-6a1 1 0 011-1h2a1 1 0 011 1v6m-4 0v-6a1 1 0 011-1h2a1 1 0 011 1v6" />
                </svg>
                <span class="font-bold text-2xl text-gray-900">Romano Sandoval</span>
            </a>
            <div class="hidden md:flex items-center space-x-6 text-lg">
                <a href="#servicios" class="text-gray-600 hover:text-indigo-600 transition-colors duration-300">Servicios</a>
                <button onclick="openModal()" class="text-gray-600 hover:text-indigo-600 transition-colors duration-300">Reserva</button>
                <a href="#contacto" class="text-gray-600 hover:text-indigo-600 transition-colors duration-300">Contacto</a>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="relative bg-center bg-cover h-screen flex items-center justify-center p-6" style="background-image: url('https://placehold.co/1920x1080/000000/FFFFFF?text=Transporte+Ejecutivo');">
        <div class="absolute inset-0 bg-black opacity-60"></div>
        <div class="relative z-10 text-center text-white max-w-2xl">
            <h1 class="text-4xl sm:text-5xl md:text-6xl font-extrabold leading-tight tracking-tight mb-4">
                Transporte Ejecutivo y al Aeropuerto
            </h1>
            <p class="text-lg sm:text-xl md:text-2xl font-light mb-8">
                Viaja con estilo, seguridad y puntualidad. Tu destino, nuestra prioridad.
            </p>
            <button onclick="openModal()" class="inline-block bg-indigo-600 text-white font-bold py-3 px-8 rounded-full shadow-lg hover:bg-indigo-700 transition-transform transform hover:scale-105">
                Reserva Ahora
            </button>
        </div>
    </section>

    <!-- Services Section -->
    <section id="servicios" class="py-16 md:py-24 px-6">
        <div class="container mx-auto">
            <h2 class="text-3xl sm:text-4xl font-bold text-center mb-12">Nuestros Servicios</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 md:gap-12">
                <!-- Service 1: Airport Transfer -->
                <div class="bg-white p-8 rounded-2xl shadow-xl flex flex-col items-center text-center hover:shadow-2xl transition-shadow duration-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16 text-indigo-600 mb-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8" />
                    </svg>
                    <h3 class="text-2xl font-bold mb-2">Transporte al Aeropuerto</h3>
                    <p class="text-gray-600 leading-relaxed">
                        Viajes puntuales y sin estrés hacia y desde el aeropuerto. Monitoreamos tu vuelo para asegurar una recogida perfecta, sin importar retrasos o cambios de horario.
                    </p>
                </div>
                <!-- Service 2: Executive Transport -->
                <div class="bg-white p-8 rounded-2xl shadow-xl flex flex-col items-center text-center hover:shadow-2xl transition-shadow duration-300">
                    <!-- New Car Icon for Executive Transport -->
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16 text-indigo-600 mb-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M19 17.5a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0z" />
                        <path d="M9 17.5a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0z" />
                        <path d="M21 9h-2l-2-4H7L5 9H3c-1.1 0-2 .9-2 2v6h20v-6c0-1.1-.9-2-2-2z" />
                        <path d="M4 14h16" />
                    </svg>
                    <h3 class="text-2xl font-bold mb-2">Transporte Ejecutivo</h3>
                    <p class="text-gray-600 leading-relaxed">
                        Servicio de transporte de primera clase para tus reuniones de negocios o eventos especiales. Coches cómodos y choferes profesionales para una experiencia de viaje inigualable.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contacto" class="py-16 md:py-24 px-6">
        <div class="container mx-auto">
            <h2 class="text-3xl sm:text-4xl font-bold text-center mb-12">Contáctanos</h2>
            <div class="bg-white p-8 md:p-12 rounded-2xl shadow-xl max-w-2xl mx-auto text-center">
                <p class="text-lg text-gray-600 mb-6">
                    ¿Tienes alguna pregunta o necesitas un servicio personalizado? Contáctame directamente para recibir atención rápida.
                </p>
                <!-- Contact Info -->
                <div class="space-y-4 mb-8 text-left inline-block">
                    <p class="flex items-center space-x-3 text-lg">
                        <!-- User Icon -->
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-indigo-600" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2"></path>
                            <circle cx="12" cy="7" r="4"></circle>
                        </svg>
                        <span>Romano Sandoval Lizano</span>
                    </p>
                    <p class="flex items-center space-x-3 text-lg">
                        <!-- New Phone Icon -->
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-indigo-600" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <rect width="14" height="20" x="5" y="2" rx="2" ry="2" />
                            <path d="M12 18h.01" />
                        </svg>
                        <a href="tel:+50664499462" class="text-indigo-600 hover:text-indigo-800 transition-colors duration-300">+506 6449-9462</a>
                    </p>
                    <p class="flex items-center space-x-3 text-lg">
                        <!-- Email Icon -->
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-indigo-600" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z" />
                            <polyline points="22,6 12,13 2,6" />
                        </svg>
                        <a href="mailto:romasl87@gmail.com" class="text-indigo-600 hover:text-indigo-800 transition-colors duration-300">romasl87@gmail.com</a>
                    </p>
                </div>

                <!-- Inquiry Button -->
                <a href="https://wa.me/50664499462?text=Hola,%20me%20gustaría%20obtener%20más%20información%20sobre%20los%20servicios%20de%20transporte%20ejecutivo." target="_blank" class="inline-block bg-white text-indigo-600 font-bold py-3 px-8 rounded-full shadow-lg border-2 border-indigo-600 hover:bg-indigo-600 hover:text-white transition-colors duration-300">
                    Hacer una consulta
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-8 px-6">
        <div class="container mx-auto text-center text-sm">
            <p>&copy; 2024 Romano Sandoval Transportes. Todos los derechos reservados.</p>
        </div>
    </footer>

    <!-- Reservation Modal -->
    <div id="reservationModal" class="hidden fixed inset-0 z-50 flex items-center justify-center p-4 modal-backdrop">
        <div class="bg-white p-8 md:p-12 rounded-2xl shadow-xl max-w-2xl mx-auto w-full relative modal-content max-h-[90vh] overflow-y-auto">
            <button onclick="closeModal()" class="absolute top-4 right-4 text-gray-400 hover:text-gray-600 transition-colors duration-200">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                </svg>
            </button>
            <h2 class="text-3xl sm:text-4xl font-bold text-center mb-6">Agenda tu Servicio</h2>
            <p class="text-lg text-gray-600 mb-6 text-center">
                Completa los datos para tu reserva. Se abrirá un evento de Google Calendar para que confirmes los detalles.
            </p>
            <form id="reservationForm" class="grid grid-cols-1 md:grid-cols-2 gap-6" onsubmit="event.preventDefault(); createCalendarEvent();">
                <div>
                    <label for="service" class="block text-gray-700 font-medium mb-2">Tipo de Servicio</label>
                    <select id="service" name="service" required class="w-full p-3 rounded-lg border-2 border-gray-300 focus:outline-none focus:ring-2 focus:ring-indigo-500 transition-colors duration-300">
                        <option value="Transporte al Aeropuerto">Transporte al Aeropuerto</option>
                        <option value="Transporte Ejecutivo">Transporte Ejecutivo</option>
                    </select>
                </div>
                <div>
                    <label for="name" class="block text-gray-700 font-medium mb-2">Tu Nombre Completo</label>
                    <input type="text" id="name" name="name" required class="w-full p-3 rounded-lg border-2 border-gray-300 focus:outline-none focus:ring-2 focus:ring-indigo-500 transition-colors duration-300">
                </div>
                <div>
                    <label for="date" class="block text-gray-700 font-medium mb-2">Fecha</label>
                    <input type="date" id="date" name="date" required class="w-full p-3 rounded-lg border-2 border-gray-300 focus:outline-none focus:ring-2 focus:ring-indigo-500 transition-colors duration-300">
                </div>
                <div>
                    <label for="time" class="block text-gray-700 font-medium mb-2">Hora</label>
                    <input type="time" id="time" name="time" required class="w-full p-3 rounded-lg border-2 border-gray-300 focus:outline-none focus:ring-2 focus:ring-indigo-500 transition-colors duration-300">
                </div>
                <div class="md:col-span-2">
                    <label for="pickupLocation" class="block text-gray-700 font-medium mb-2">Lugar de Recogida</label>
                    <input type="text" id="pickupLocation" name="pickupLocation" required class="w-full p-3 rounded-lg border-2 border-gray-300 focus:outline-none focus:ring-2 focus:ring-indigo-500 transition-colors duration-300">
                </div>
                <div class="md:col-span-2">
                    <label for="dropoffLocation" class="block text-gray-700 font-medium mb-2">Lugar de Destino</label>
                    <input type="text" id="dropoffLocation" name="dropoffLocation" required class="w-full p-3 rounded-lg border-2 border-gray-300 focus:outline-none focus:ring-2 focus:ring-indigo-500 transition-colors duration-300">
                </div>
                <div class="md:col-span-2">
                    <label for="comments" class="block text-gray-700 font-medium mb-2">Comentarios (Opcional)</label>
                    <textarea id="comments" name="comments" rows="3" class="w-full p-3 rounded-lg border-2 border-gray-300 focus:outline-none focus:ring-2 focus:ring-indigo-500 transition-colors duration-300"></textarea>
                </div>
                <div class="md:col-span-2 text-center mt-4">
                    <button type="submit" class="w-full bg-indigo-600 text-white font-bold py-3 px-8 rounded-full shadow-lg hover:bg-indigo-700 transition-transform transform hover:scale-105">
                        Reservar
                    </button>
                </div>
            </form>
        </div>
    </div>

    <script>
        // Función para abrir la ventana modal de reserva
        function openModal() {
            document.getElementById('reservationModal').classList.remove('hidden');
        }

        // Función para cerrar la ventana modal de reserva
        function closeModal() {
            document.getElementById('reservationModal').classList.add('hidden');
        }

        function createCalendarEvent() {
            const form = document.getElementById('reservationForm');
            const service = form.service.value;
            const name = form.name.value;
            const date = form.date.value;
            const time = form.time.value;
            const pickupLocation = form.pickupLocation.value;
            const dropoffLocation = form.dropoffLocation.value;
            const comments = form.comments.value;

            // Formato de fecha para Google Calendar: YYYYMMDDTHHMMSS
            const dateTime = new Date(`${date}T${time}:00`);
            const year = dateTime.getFullYear();
            const month = String(dateTime.getMonth() + 1).padStart(2, '0');
            const day = String(dateTime.getDate()).padStart(2, '0');
            const hours = String(dateTime.getHours()).padStart(2, '0');
            const minutes = String(dateTime.getMinutes()).padStart(2, '0');
            const formattedDate = `${year}${month}${day}T${hours}${minutes}00`;
            
            // Título del evento
            const title = `Reserva de ${service} - ${name}`;

            // Detalles del evento
            const details = `
                Servicio: ${service}
                Cliente: ${name}
                Fecha: ${date}
                Hora: ${time}
                Lugar de Recogida: ${pickupLocation}
                Lugar de Destino: ${dropoffLocation}
                Comentarios: ${comments}
            `;

            const googleCalendarUrl = `https://calendar.google.com/calendar/render?action=TEMPLATE&text=${encodeURIComponent(title)}&dates=${formattedDate}/${formattedDate}&details=${encodeURIComponent(details)}&sf=true`;
            
            // Abre la URL en una nueva pestaña
            window.open(googleCalendarUrl, '_blank');

            // Ocultar la modal después de enviar
            closeModal();
        }
    </script>
</body>
</html>
