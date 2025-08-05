<!DOCTYPE html>
<html lang="es" class="">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MiApp - DI</title>
    
    <!-- PWA Manifest and Theme Color -->
    <meta name="theme-color" content="#A855F7">
    <link rel="manifest" href="manifest.json">
    <link rel="apple-touch-icon" href="icon-192x192.png">

    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

    <!-- Feather Icons for cleaner icons -->
    <script src="https://unpkg.com/feather-icons"></script>

    <style>
        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            -webkit-tap-highlight-color: transparent;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .fade-in { animation: fadeIn 0.4s ease-in-out; }
        .task-completed { text-decoration: line-through; opacity: 0.6; }
        .gym-day { transition: all 0.2s ease-in-out; }
        .gym-day.completed { background-color: #10B981; transform: scale(1.1); }
        .gym-day.current {
            border: 2px solid #A855F7; /* purple-500 */
            animation: pulse-border 2s infinite;
        }
        @keyframes pulse-border {
            0% { box-shadow: 0 0 0 0 rgba(168, 85, 247, 0.4); }
            70% { box-shadow: 0 0 0 5px rgba(168, 85, 247, 0); }
            100% { box-shadow: 0 0 0 0 rgba(168, 85, 247, 0); }
        }
        /* Style for bottom nav icons when active */
        .bottom-nav-button.active {
            color: #A855F7; /* purple-500 */
        }
        html.dark .bottom-nav-button.active {
            color: #F472B6; /* pink-400 */
        }
    </style>
    <script>
        tailwind.config = { darkMode: 'class' }
    </script>
</head>
<body class="bg-gray-200 dark:bg-gray-900 transition-colors duration-300">

    <!-- Main App Container -->
    <div class="container mx-auto max-w-sm h-screen flex flex-col bg-gray-100 dark:bg-gray-800 shadow-2xl overflow-hidden">

        <!-- Header Section -->
        <header class="bg-gradient-to-br from-purple-500 to-pink-500 dark:from-purple-600 dark:to-pink-600 text-white p-6 text-center rounded-b-3xl shadow-lg">
            <div class="flex justify-between items-center mb-4">
                <div class="text-sm font-bold" id="current-time">09:41</div>
                <div class="flex items-center gap-2 text-sm">
                    <span id="battery-level">95%</span>
                    <i data-feather="battery" class="w-5 h-5"></i>
                </div>
            </div>
            <img src="https://placehold.co/100x100/fecaca/333333?text=DI" alt="Foto de Perfil" class="w-24 h-24 rounded-full mx-auto border-4 border-white/50 mb-4">
            <h1 class="text-2xl font-bold">¡Hola, PILARCITA! 👋</h1>
            <p class="text-sm opacity-80" id="header-subtitle">¡Lista para un día increíble!</p>
        </header>

        <!-- Main Content Area -->
        <main class="flex-grow flex flex-col overflow-hidden">
            <div class="flex-grow p-5 overflow-y-auto bg-gray-50 dark:bg-gray-900">
                
                <!-- Home/Dashboard Page -->
                <div id="dashboard" class="tab-content active fade-in space-y-4">
                    <h2 class="text-xl font-bold text-gray-800 dark:text-white">Panel de Control</h2>
                    <!-- Dynamic content will be injected here -->
                    <div id="dashboard-reminders"></div>
                    <div id="dashboard-tasks"></div>
                    <div id="dashboard-gym"></div>
                    <div id="dashboard-notes"></div>
                    <div id="dashboard-achievements"></div>
                </div>

                <!-- Tasks Page -->
                <div id="tasks" class="tab-content hidden fade-in">
                    <h2 class="text-xl font-bold text-gray-800 dark:text-white mb-4">Mis Tareas</h2>
                    <div class="bg-white dark:bg-gray-800 p-4 rounded-xl shadow-md">
                        <input id="new-task-input" type="text" placeholder="Ej: Estudiar para examen de Derecho Civil" class="w-full p-3 bg-gray-100 dark:bg-gray-700 border-2 border-transparent focus:border-purple-500 rounded-lg outline-none transition-colors">
                        <button id="add-task-btn" class="w-full mt-3 bg-purple-500 hover:bg-purple-600 text-white font-bold py-2 px-4 rounded-lg transition-transform transform active:scale-95">Añadir Tarea</button>
                    </div>
                    <h3 class="text-lg font-bold text-gray-800 dark:text-white mt-6 mb-3">Pendientes</h3>
                    <div id="task-list" class="space-y-3"></div>
                </div>

                <!-- Reminders Page -->
                <div id="reminders" class="tab-content hidden fade-in">
                    <h2 class="text-xl font-bold text-gray-800 dark:text-white mb-4">Mis Recordatorios</h2>
                    <div class="bg-white dark:bg-gray-800 p-4 rounded-xl shadow-md">
                        <div class="space-y-3">
                            <input id="new-reminder-text" type="text" placeholder="¿Qué necesitas recordar?" class="w-full p-3 bg-gray-100 dark:bg-gray-700 border-2 border-transparent focus:border-purple-500 rounded-lg outline-none transition-colors">
                            <input id="new-reminder-datetime" type="datetime-local" class="w-full p-3 bg-gray-100 dark:bg-gray-700 border-2 border-transparent focus:border-purple-500 rounded-lg outline-none transition-colors text-gray-700 dark:text-gray-300">
                        </div>
                        <button id="add-reminder-btn" class="w-full mt-3 bg-purple-500 hover:bg-purple-600 text-white font-bold py-2 px-4 rounded-lg transition-transform transform active:scale-95">Programar Recordatorio</button>
                    </div>
                    <h3 class="text-lg font-bold text-gray-800 dark:text-white mt-6 mb-3">Próximos</h3>
                    <div id="reminders-list" class="space-y-3"></div>
                </div>
                
                <!-- Gym Motivation Page -->
                <div id="motivation" class="tab-content hidden fade-in">
                    <h2 class="text-xl font-bold text-gray-800 dark:text-white mb-2">Motivación Gym</h2>
                    <div class="bg-white dark:bg-gray-800 p-4 rounded-xl shadow-md">
                        <div class="flex justify-between items-center mb-3">
                            <h3 class="font-bold text-gray-800 dark:text-white">Reto 365 Días</h3>
                            <span class="text-sm font-bold text-purple-500"><span id="gym-days-count">0</span>/365</span>
                        </div>
                        <div id="gym-grid" class="grid grid-cols-12 gap-1.5"></div>
                    </div>
                     <div class="bg-white dark:bg-gray-800 p-5 rounded-xl shadow-md mt-5">
                        <h3 class="font-bold text-gray-800 dark:text-white mb-2 flex items-center gap-2"><i data-feather="zap" class="w-5 h-5 text-yellow-400"></i>Frase del Día</h3>
                        <p id="motivation-quote" class="text-sm text-gray-600 dark:text-gray-300 italic">"La disciplina es el puente entre las metas y los logros."</p>
                    </div>
                </div>

                <!-- Notes Page -->
                <div id="notes" class="tab-content hidden fade-in">
                     <h2 class="text-xl font-bold text-gray-800 dark:text-white mb-4">Mis Notas</h2>
                     <div class="bg-white dark:bg-gray-800 p-4 rounded-xl shadow-md mb-5">
                        <textarea id="quick-note-input" placeholder="Anota tus ideas, campeona..." class="w-full p-3 h-24 bg-gray-100 dark:bg-gray-700 border-2 border-transparent focus:border-purple-500 rounded-lg outline-none transition-colors"></textarea>
                        <button id="save-note-btn" class="w-full mt-3 bg-purple-500 hover:bg-purple-600 text-white font-bold py-2 px-4 rounded-lg transition-transform transform active:scale-95">Guardar Nota</button>
                    </div>
                    <div id="notes-list" class="space-y-3"></div>
                </div>

                <!-- Achievements Page -->
                <div id="achievements" class="tab-content hidden fade-in">
                    <h2 class="text-xl font-bold text-gray-800 dark:text-white mb-4">Mis Logros</h2>
                    <div id="achievements-list" class="space-y-3"></div>
                </div>

            </div>
        </main>

        <!-- Bottom Navigation Bar -->
        <footer class="bg-white dark:bg-gray-800 border-t border-gray-200 dark:border-gray-700 shadow-inner p-1 flex justify-around rounded-t-3xl z-10">
            <button data-tab-button="dashboard" class="bottom-nav-button active flex-1 flex flex-col items-center justify-center p-2 rounded-lg text-xs"><i data-feather="home" class="w-5 h-5 mb-1"></i>Inicio</button>
            <button data-tab-button="tasks" class="bottom-nav-button flex-1 flex flex-col items-center justify-center p-2 rounded-lg text-xs"><i data-feather="check-square" class="w-5 h-5 mb-1"></i>Tareas</button>
            <button data-tab-button="reminders" class="bottom-nav-button flex-1 flex flex-col items-center justify-center p-2 rounded-lg text-xs"><i data-feather="bell" class="w-5 h-5 mb-1"></i>Alertas</button>
            <button data-tab-button="motivation" class="bottom-nav-button flex-1 flex flex-col items-center justify-center p-2 rounded-lg text-xs"><i data-feather="heart" class="w-5 h-5 mb-1"></i>Gym</button>
            <button data-tab-button="notes" class="bottom-nav-button flex-1 flex flex-col items-center justify-center p-2 rounded-lg text-xs"><i data-feather="edit-3" class="w-5 h-5 mb-1"></i>Notas</button>
            <button data-tab-button="achievements" class="bottom-nav-button flex-1 flex flex-col items-center justify-center p-2 rounded-lg text-xs"><i data-feather="award" class="w-5 h-5 mb-1"></i>Logros</button>
        </footer>
    </div>

    <!-- Notification / Toast Element -->
    <div id="notification" class="fixed bottom-24 left-1/2 -translate-x-1/2 bg-gray-900 dark:bg-white text-white dark:text-gray-900 text-sm font-semibold py-3 px-6 rounded-full shadow-lg opacity-0 translate-y-4 transition-all duration-300 z-50"></div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            
            // --- DATABASE & USER DATA ---
            const APP_STORAGE_KEY = 'dianaApp_userData_v3'; // Version updated

            const defaultUserData = {
                name: "DI",
                nicknames: ["DI", "PILARCITA"],
                tasks: [
                    { id: 1, text: "Leer jurisprudencia ambiental", completed: false, timestamp: "04/08/2025, 10:00" },
                ],
                reminders: [],
                notes: [],
                gymLog: [],
                streak: 7,
                achievements: [
                    { id: 'first_gym', title: '¡A empezar!', description: 'Completa tu primer día de gym.', unlocked: false, icon: 'activity' },
                    { id: 'week_gym', title: 'Constancia es Poder', description: 'Entrena 7 días.', unlocked: false, icon: 'bar-chart-2' },
                    { id: 'law_task', title: 'Futura Abogada', description: 'Completa una tarea de Derecho.', unlocked: false, icon: 'briefcase' },
                    { id: 'first_note', title: 'Anotadora', description: 'Guarda tu primera nota.', unlocked: false, icon: 'edit' },
                    { id: 'month_gym', title: 'Hábito Creado', description: 'Entrena por un mes (30 días).', unlocked: false, icon: 'award' }
                ]
            };

            let userData = {};

            // --- ELEMENT SELECTORS ---
            const timeEl = document.getElementById('current-time');
            const notificationEl = document.getElementById('notification');
            const headerSubtitleEl = document.getElementById('header-subtitle');
            const tabContents = document.querySelectorAll('.tab-content');
            const bottomNavButtons = document.querySelectorAll('.bottom-nav-button');
            const taskListEl = document.getElementById('task-list');
            const newTaskInputEl = document.getElementById('new-task-input');
            const notesListEl = document.getElementById('notes-list');
            const quickNoteInputEl = document.getElementById('quick-note-input');
            const gymGridEl = document.getElementById('gym-grid');
            const remindersListEl = document.getElementById('reminders-list');
            const newReminderTextInput = document.getElementById('new-reminder-text');
            const newReminderDatetimeInput = document.getElementById('new-reminder-datetime');

            // --- INITIALIZATION ---
            function init() {
                loadData();
                setupTheme();
                updateTime();
                setInterval(updateTime, 10000);
                setInterval(checkReminders, 30000);
                
                renderAll();
                setupEventListeners();
                
                showNotification(`¡Vamos con todo, ${userData.nicknames[1]}! 🚀`, 2000);
            }

            // --- DATA PERSISTENCE ---
            function loadData() {
                const savedData = localStorage.getItem(APP_STORAGE_KEY);
                userData = savedData ? JSON.parse(savedData) : JSON.parse(JSON.stringify(defaultUserData));
            }

            function saveData() {
                localStorage.setItem(APP_STORAGE_KEY, JSON.stringify(userData));
            }

            // --- RENDER FUNCTIONS ---
            function renderAll() {
                renderDashboard();
                renderTasks();
                renderNotes();
                renderAchievements();
                renderGymGrid();
                renderReminders();
                if(document.getElementById('streak-count')) {
                    document.getElementById('streak-count').textContent = userData.streak;
                }
                feather.replace();
            }

            function renderDashboard() {
                const remindersContainer = document.getElementById('dashboard-reminders');
                const tasksContainer = document.getElementById('dashboard-tasks');
                const gymContainer = document.getElementById('dashboard-gym');
                const notesContainer = document.getElementById('dashboard-notes');
                const achievementsContainer = document.getElementById('dashboard-achievements');

                // 1. Render Reminders
                const upcomingReminder = [...userData.reminders].sort((a, b) => new Date(a.datetime) - new Date(b.datetime))[0];
                remindersContainer.innerHTML = `
                    <div class="bg-white dark:bg-gray-800 p-4 rounded-xl shadow-md">
                        <h3 class="font-bold text-gray-800 dark:text-white mb-2 flex items-center gap-2"><i data-feather="bell" class="w-5 h-5 text-purple-500"></i>Próxima Alerta</h3>
                        ${upcomingReminder ? `
                            <p class="text-sm text-gray-600 dark:text-gray-300"><strong>${upcomingReminder.text}</strong></p>
                            <p class="text-xs text-purple-500">${new Date(upcomingReminder.datetime).toLocaleString('es-ES', { dateStyle: 'full', timeStyle: 'short' })}</p>
                        ` : `
                            <p class="text-sm text-gray-500 dark:text-gray-400">No tienes alertas programadas.</p>
                        `}
                    </div>`;

                // 2. Render Tasks
                const pendingTasks = userData.tasks.filter(t => !t.completed).slice(0, 3);
                tasksContainer.innerHTML = `
                    <div class="bg-white dark:bg-gray-800 p-4 rounded-xl shadow-md">
                        <h3 class="font-bold text-gray-800 dark:text-white mb-2 flex items-center gap-2"><i data-feather="check-square" class="w-5 h-5 text-green-500"></i>Tareas Pendientes</h3>
                        ${pendingTasks.length > 0 ? `
                            <ul class="space-y-2">
                                ${pendingTasks.map(task => `<li class="text-sm text-gray-600 dark:text-gray-300">${task.text}</li>`).join('')}
                            </ul>
                        ` : `
                            <p class="text-sm text-gray-500 dark:text-gray-400">¡Ninguna tarea pendiente! ¡Excelente!</p>
                        `}
                    </div>`;

                // 3. Render Gym
                gymContainer.innerHTML = `
                    <div class="bg-white dark:bg-gray-800 p-4 rounded-xl shadow-md">
                        <h3 class="font-bold text-gray-800 dark:text-white mb-2 flex items-center gap-2"><i data-feather="heart" class="w-5 h-5 text-red-500"></i>Progreso Gym</h3>
                        <div class="w-full bg-gray-200 rounded-full h-2.5 dark:bg-gray-700">
                            <div class="bg-green-500 h-2.5 rounded-full" style="width: ${ (userData.gymLog.length / 365) * 100}%"></div>
                        </div>
                        <p class="text-center text-sm mt-2 text-gray-600 dark:text-gray-400">${userData.gymLog.length} de 365 días completados.</p>
                    </div>`;

                // 4. Render Notes
                const latestNote = userData.notes[0];
                notesContainer.innerHTML = `
                    <div class="bg-white dark:bg-gray-800 p-4 rounded-xl shadow-md">
                        <h3 class="font-bold text-gray-800 dark:text-white mb-2 flex items-center gap-2"><i data-feather="edit-3" class="w-5 h-5 text-blue-500"></i>Última Nota</h3>
                        ${latestNote ? `
                            <p class="text-sm text-gray-600 dark:text-gray-300 truncate">${latestNote.text}</p>
                            <p class="text-xs text-gray-400 mt-1">${latestNote.timestamp}</p>
                        ` : `
                            <p class="text-sm text-gray-500 dark:text-gray-400">Aún no has escrito notas.</p>
                        `}
                    </div>`;

                // 5. Render Achievements
                const nextAchievement = userData.achievements.find(a => !a.unlocked);
                achievementsContainer.innerHTML = `
                    <div class="bg-white dark:bg-gray-800 p-4 rounded-xl shadow-md">
                        <h3 class="font-bold text-gray-800 dark:text-white mb-2 flex items-center gap-2"><i data-feather="award" class="w-5 h-5 text-yellow-500"></i>Próximo Logro</h3>
                        ${nextAchievement ? `
                            <p class="text-sm text-gray-600 dark:text-gray-300"><strong>${nextAchievement.title}:</strong> ${nextAchievement.description}</p>
                        ` : `
                            <p class="text-sm text-gray-500 dark:text-gray-400">¡Has desbloqueado todos los logros!</p>
                        `}
                    </div>`;
                feather.replace();
            }
            
            function renderTasks() {
                taskListEl.innerHTML = userData.tasks.length > 0 ? userData.tasks.map(task => `
                    <div class="flex items-center justify-between bg-white dark:bg-gray-800 p-3 rounded-lg shadow-sm">
                        <div>
                            <p class="font-semibold text-gray-800 dark:text-white ${task.completed ? 'task-completed' : ''}">${task.text}</p>
                            <p class="text-xs text-gray-400">${task.timestamp}</p>
                        </div>
                        <div class="flex gap-2">
                            <button data-task-id="${task.id}" class="toggle-task-btn p-2 text-green-500 hover:bg-green-100 dark:hover:bg-gray-700 rounded-md"><i data-feather="${task.completed ? 'check-circle' : 'circle'}" class="w-5 h-5 pointer-events-none"></i></button>
                            <button data-task-id="${task.id}" class="delete-task-btn p-2 text-red-500 hover:bg-red-100 dark:hover:bg-gray-700 rounded-md"><i data-feather="trash-2" class="w-5 h-5 pointer-events-none"></i></button>
                        </div>
                    </div>`).join('') : `<p class="text-center text-gray-500 dark:text-gray-400">¡Sin pendientes! Añade una tarea.</p>`;
                feather.replace();
            }

            function renderReminders() {
                const sortedReminders = [...userData.reminders].sort((a, b) => new Date(a.datetime) - new Date(b.datetime));
                remindersListEl.innerHTML = sortedReminders.length > 0 ? sortedReminders.map(reminder => {
                    const reminderDate = new Date(reminder.datetime);
                    const formattedDate = reminderDate.toLocaleString('es-ES', { dateStyle: 'medium', timeStyle: 'short' });
                    return `
                    <div class="flex items-center justify-between bg-white dark:bg-gray-800 p-3 rounded-lg shadow-sm">
                        <div>
                            <p class="font-semibold text-gray-800 dark:text-white">${reminder.text}</p>
                            <p class="text-xs text-purple-500 dark:text-pink-400">${formattedDate}</p>
                        </div>
                        <button data-reminder-id="${reminder.id}" class="delete-reminder-btn p-2 text-red-500 hover:bg-red-100 dark:hover:bg-gray-700 rounded-md"><i data-feather="trash-2" class="w-5 h-5 pointer-events-none"></i></button>
                    </div>`;
                }).join('') : `<p class="text-center text-gray-500 dark:text-gray-400">No hay recordatorios programados.</p>`;
                feather.replace();
            }

            function renderNotes() {
                notesListEl.innerHTML = userData.notes.length > 0 ? userData.notes.map(note => `
                    <div class="bg-white dark:bg-gray-800 p-4 rounded-lg shadow-sm">
                        <p class="text-gray-700 dark:text-gray-300 mb-2 whitespace-pre-wrap">${note.text}</p>
                        <div class="flex justify-between items-center text-xs text-gray-400">
                            <span>${note.timestamp}</span>
                            <button data-note-id="${note.id}" class="delete-note-btn p-1 text-red-500 hover:bg-red-100 dark:hover:bg-gray-700 rounded-md"><i data-feather="trash" class="w-4 h-4 pointer-events-none"></i></button>
                        </div>
                    </div>`).join('') : `<p class="text-center text-gray-500 dark:text-gray-400">Aún no has guardado notas.</p>`;
                feather.replace();
            }

            function renderAchievements() {
                 document.getElementById('achievements-list').innerHTML = userData.achievements.map(ach => `
                    <div class="flex items-center gap-4 bg-white dark:bg-gray-800 p-4 rounded-lg shadow-sm ${ach.unlocked ? 'border-l-4 border-green-500' : 'opacity-60'}">
                        <i data-feather="${ach.icon}" class="w-8 h-8 ${ach.unlocked ? 'text-green-500' : 'text-gray-500'}"></i>
                        <div>
                            <h4 class="font-bold text-gray-800 dark:text-white">${ach.title}</h4>
                            <p class="text-sm text-gray-600 dark:text-gray-400">${ach.description}</p>
                        </div>
                    </div>`).join('');
                feather.replace();
            }

            function renderGymGrid() {
                const gymDaysCountEl = document.getElementById('gym-days-count');
                const now = new Date();
                const start = new Date(now.getFullYear(), 0, 0);
                const diff = now - start;
                const oneDay = 1000 * 60 * 60 * 24;
                const dayOfYear = Math.floor(diff / oneDay) - 1;

                gymGridEl.innerHTML = '';
                for (let i = 0; i < 365; i++) {
                    const dayDiv = document.createElement('div');
                    dayDiv.classList.add('gym-day', 'h-3', 'w-full', 'bg-gray-200', 'dark:bg-gray-700', 'rounded-sm', 'cursor-pointer');
                    dayDiv.dataset.dayIndex = i;
                    if (userData.gymLog.includes(i)) {
                        dayDiv.classList.add('completed');
                    }
                    if (i === dayOfYear) {
                        dayDiv.classList.add('current');
                    }
                    gymGridEl.appendChild(dayDiv);
                }
                gymDaysCountEl.textContent = userData.gymLog.length;
            }


            // --- EVENT LISTENERS ---
            function setupEventListeners() {
                bottomNavButtons.forEach(button => button.addEventListener('click', handleTabSwitch));
                document.getElementById('add-task-btn').addEventListener('click', addTask);
                document.getElementById('save-note-btn').addEventListener('click', saveNote);
                document.getElementById('add-reminder-btn').addEventListener('click', addReminder);
                taskListEl.addEventListener('click', handleTaskListClick);
                notesListEl.addEventListener('click', handleDeleteNoteClick);
                remindersListEl.addEventListener('click', handleDeleteReminderClick);
                gymGridEl.addEventListener('click', handleGymGridClick);
            }
            
            function handleTabSwitch(event) {
                const targetTab = event.currentTarget.dataset.tabButton;
                tabContents.forEach(content => content.classList.add('hidden'));
                bottomNavButtons.forEach(btn => btn.classList.remove('active'));
                
                document.getElementById(targetTab).classList.remove('hidden');
                event.currentTarget.classList.add('active');
                headerSubtitleEl.textContent = `Estás en: ${targetTab.charAt(0).toUpperCase() + targetTab.slice(1)}`;
            }

            function handleTaskListClick(event) {
                const button = event.target.closest('button');
                if (!button) return;
                const taskId = button.dataset.taskId;
                if (button.matches('.toggle-task-btn')) toggleTask(parseInt(taskId));
                if (button.matches('.delete-task-btn')) deleteTask(parseInt(taskId));
            }
            
            function handleDeleteNoteClick(event) {
                const button = event.target.closest('button');
                if (button && button.matches('.delete-note-btn')) {
                    deleteNote(parseInt(button.dataset.noteId));
                }
            }

            function handleDeleteReminderClick(event) {
                const button = event.target.closest('button');
                if (button && button.matches('.delete-reminder-btn')) {
                    deleteReminder(parseInt(button.dataset.reminderId));
                }
            }

            function handleGymGridClick(event) {
                const dayIndex = event.target.dataset.dayIndex;
                if (dayIndex !== undefined) {
                    toggleGymDay(parseInt(dayIndex));
                }
            }

            // --- CORE LOGIC ---
            function addReminder() {
                const text = newReminderTextInput.value.trim();
                const datetime = newReminderDatetimeInput.value;
                if (!text || !datetime) {
                    showNotification("Por favor, completa ambos campos.", 3000);
                    return;
                }
                userData.reminders.push({ id: Date.now(), text, datetime });
                newReminderTextInput.value = '';
                newReminderDatetimeInput.value = '';
                saveData();
                renderAll();
                showNotification("Recordatorio programado.", 3000);
            }

            function deleteReminder(reminderId) {
                userData.reminders = userData.reminders.filter(r => r.id !== reminderId);
                saveData();
                renderAll();
                showNotification("Recordatorio eliminado.", 2000);
            }
            
            function checkReminders() {
                const now = new Date();
                const dueReminders = userData.reminders.filter(r => new Date(r.datetime) <= now);

                if (dueReminders.length > 0) {
                    dueReminders.forEach(reminder => {
                        showNotification(`¡ALARMA! ${reminder.text}`, 5000);
                        userData.reminders = userData.reminders.filter(r => r.id !== reminder.id);
                    });
                    saveData();
                    renderAll();
                }
            }

            function addTask() {
                const text = newTaskInputEl.value.trim();
                if (text) {
                    const now = new Date();
                    userData.tasks.unshift({ 
                        id: Date.now(), 
                        text, 
                        completed: false,
                        timestamp: now.toLocaleString('es-ES', { day: '2-digit', month: '2-digit', year: 'numeric', hour: '2-digit', minute: '2-digit' })
                    });
                    newTaskInputEl.value = '';
                    saveData();
                    renderAll();
                    showNotification('¡Tarea añadida con éxito!');
                }
            }
            function toggleTask(taskId) {
                const task = userData.tasks.find(t => t.id === taskId);
                if (task) {
                    task.completed = !task.completed;
                    if(task.completed) showNotification('¡Bien hecho, PILARCITA!');
                    saveData();
                    renderAll();
                }
            }
            function deleteTask(taskId) {
                userData.tasks = userData.tasks.filter(t => t.id !== taskId);
                saveData();
                renderAll();
                showNotification('Tarea eliminada.', 2000);
            }
            function saveNote() {
                const text = quickNoteInputEl.value.trim();
                if (text) {
                    const now = new Date();
                    const newNote = {
                        id: Date.now(),
                        text: text,
                        timestamp: now.toLocaleString('es-ES', { day: '2-digit', month: '2-digit', year: 'numeric', hour: '2-digit', minute: '2-digit' })
                    };
                    userData.notes.unshift(newNote);
                    quickNoteInputEl.value = '';
                    saveData();
                    renderAll();
                    showNotification('Nota guardada.');
                }
            }
            function deleteNote(noteId) {
                userData.notes = userData.notes.filter(n => n.id !== noteId);
                saveData();
                renderAll();
                showNotification('Nota eliminada.', 2000);
            }
            function toggleGymDay(dayIndex) {
                const logIndex = userData.gymLog.indexOf(dayIndex);
                if (logIndex > -1) {
                    userData.gymLog.splice(logIndex, 1);
                } else {
                    userData.gymLog.push(dayIndex);
                }
                saveData();
                renderAll();
            }
            function checkAchievements() {
                const achievementsToUpdate = [
                    { id: 'first_gym', condition: userData.gymLog.length > 0 },
                    { id: 'week_gym', condition: userData.gymLog.length >= 7 },
                    { id: 'month_gym', condition: userData.gymLog.length >= 30 },
                    { id: 'first_note', condition: userData.notes.length > 0 },
                    { id: 'law_task', condition: userData.tasks.some(t => t.completed && t.text.toLowerCase().includes('derecho')) }
                ];

                achievementsToUpdate.forEach(achInfo => {
                    const achievement = userData.achievements.find(a => a.id === achInfo.id);
                    if (achievement && achInfo.condition && !achievement.unlocked) {
                        achievement.unlocked = true;
                        showNotification(`¡Logro: ${achievement.title}! 🏆`, 4000);
                    }
                });
                saveData();
                renderAchievements();
            }

            // --- UTILITY FUNCTIONS ---
            function updateTime() { timeEl.textContent = new Date().toLocaleTimeString('es-ES', { hour: '2-digit', minute: '2-digit' }); }
            function showNotification(message, duration = 3000) {
                clearTimeout(window.notificationTimeout);
                notificationEl.textContent = message;
                notificationEl.classList.remove('opacity-0', 'translate-y-4');
                window.notificationTimeout = setTimeout(() => notificationEl.classList.add('opacity-0', 'translate-y-4'), duration);
            }
            function setupTheme() {
                if (localStorage.theme === 'dark' || (!('theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
                    document.documentElement.classList.add('dark');
                } else {
                    document.documentElement.classList.remove('dark');
                }
            }
            function toggleTheme() {
                document.documentElement.classList.toggle('dark');
                localStorage.theme = document.documentElement.classList.contains('dark') ? 'dark' : 'light';
            }

            // --- PWA Service Worker Registration ---
            if ('serviceWorker' in navigator) {
                window.addEventListener('load', () => {
                    navigator.serviceWorker.register('./service-worker.js')
                        .then(registration => {
                            console.log('ServiceWorker registration successful with scope: ', registration.scope);
                        })
                        .catch(err => {
                            console.log('ServiceWorker registration failed: ', err);
                        });
                });
            }

            // --- START THE APP ---
            init();
        });
    </script>
</body>
</html>