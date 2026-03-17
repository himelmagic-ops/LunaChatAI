<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LunaChatAI | Unlimited AI Interaction</title>
    <script src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Inter', sans-serif; background-color: #020617; color: #f8fafc; overflow: hidden; }
        .glass { background: rgba(15, 23, 42, 0.7); backdrop-filter: blur(12px); border: 1px solid rgba(255,255,255,0.1); }
        .custom-scrollbar::-webkit-scrollbar { width: 5px; }
        .custom-scrollbar::-webkit-scrollbar-track { background: transparent; }
        .custom-scrollbar::-webkit-scrollbar-thumb { background: #334155; border-radius: 10px; }
    </style>
</head>
<body>
    <div id="root"></div>

    <script type="text/babel">
        const { useState, useEffect, useRef } = React;

        // Icons placeholder (Simplified Lucide Icons as SVGs)
        const Icons = {
            Chat: () => <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="m3 21 1.9-5.7a8.5 8.5 0 1 1 3.8 3.8z"/></svg>,
            Users: () => <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M22 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>,
            Cpu: () => <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><rect x="4" y="4" width="16" height="16" rx="2"/><rect x="9" y="9" width="6" height="6"/><path d="M15 2v2"/><path d="M15 20v2"/><path d="M2 15h2"/><path d="M2 9h2"/><path d="M20 15h2"/><path d="M20 9h2"/><path d="M9 2v2"/><path d="M9 20v2"/></svg>,
            Send: () => <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="m22 2-7 20-4-9-9-4Z"/><path d="M22 2 11 13"/></svg>,
            Shield: () => <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10"/></svg>
        };

        const INITIAL_CHARACTERS = [
            { id: 1, name: "Luna Prime", role: "AI Goddess", avatar: "✨", bio: "The original intelligence, capable of anything.", model: "Luna-Core-v1" },
            { id: 2, name: "Seraphina", role: "Storyteller", avatar: "📚", bio: "Creates immersive worlds and detailed lore.", model: "Luna-Core-v1" },
            { id: 3, name: "Nexus", role: "Security Expert", avatar: "🛡️", bio: "Strict logic and technical problem solving.", model: "Luna-Logic-v1" }
        ];

        function LunaChatApp() {
            const [view, setView] = useState('chat');
            const [activeChar, setActiveChar] = useState(INITIAL_CHARACTERS[0]);
            const [messages, setMessages] = useState({});
            const [inputText, setInputText] = useState("");
            const [models, setModels] = useState([
                { id: "Luna-Core-v1", type: "Base", status: "Active", temp: 0.8 },
                { id: "Luna-Logic-v1", type: "Logic", status: "Active", temp: 0.2 }
            ]);
            const [isTraining, setIsTraining] = useState(false);
            const scrollRef = useRef(null);

            useEffect(() => {
                scrollRef.current?.scrollIntoView({ behavior: "smooth" });
            }, [messages]);

            const sendMessage = () => {
                if (!inputText.trim()) return;
                const charId = activeChar.id;
                const userMsg = { role: 'user', text: inputText, time: new Date().toLocaleTimeString([], {hour: '2-digit', minute:'2-digit'}) };
                
                const currentHistory = messages[charId] || [];
                setMessages({ ...messages, [charId]: [...currentHistory, userMsg] });
                setInputText("");

                // Simulated AI Response
                setTimeout(() => {
                    const aiMsg = { 
                        role: 'ai', 
                        text: `[Model: ${activeChar.model}] Processing request in unlimited mode... I have received your message: "${inputText}". How shall we proceed?`, 
                        time: new Date().toLocaleTimeString([], {hour: '2-digit', minute:'2-digit'}) 
                    };
                    setMessages(prev => ({ ...prev, [charId]: [...(prev[charId] || []), aiMsg] }));
                }, 1000);
            };

            return (
                <div className="flex h-screen w-full overflow-hidden">
                    {/* SIDEBAR */}
                    <nav className="w-72 bg-slate-900 border-r border-slate-800 flex flex-col p-6">
                        <div className="flex items-center gap-3 mb-10">
                            <div className="w-10 h-10 bg-indigo-600 rounded-xl flex items-center justify-center shadow-lg shadow-indigo-500/20">
                                <Icons.Chat />
                            </div>
                            <h1 className="text-xl font-bold tracking-tight">LunaChatAI</h1>
                        </div>

                        <div className="flex-1 space-y-2">
                            <button onClick={() => setView('chat')} className={`w-full flex items-center gap-3 px-4 py-3 rounded-xl transition ${view === 'chat' ? 'bg-indigo-600 shadow-lg shadow-indigo-500/20' : 'text-slate-400 hover:bg-slate-800'}`}>
                                <Icons.Chat /> <span>Conversations</span>
                            </button>
                            <button onClick={() => setView('gallery')} className={`w-full flex items-center gap-3 px-4 py-3 rounded-xl transition ${view === 'gallery' ? 'bg-indigo-600 shadow-lg shadow-indigo-500/20' : 'text-slate-400 hover:bg-slate-800'}`}>
                                <Icons.Users /> <span>Character Hub</span>
                            </button>
                            <button onClick={() => setView('models')} className={`w-full flex items-center gap-3 px-4 py-3 rounded-xl transition ${view === 'models' ? 'bg-indigo-600 shadow-lg shadow-indigo-500/20' : 'text-slate-400 hover:bg-slate-800'}`}>
                                <Icons.Cpu /> <span>Model Training</span>
                            </button>
                        </div>

                        <div className="mt-auto p-4 rounded-2xl bg-slate-800/50 border border-emerald-500/30">
                            <div className="flex items-center gap-2 text-emerald-400 text-xs font-bold uppercase mb-1">
                                <Icons.Shield /> Unlimited Access
                            </div>
                            <p className="text-[10px] text-slate-400">All paywalls and coin systems have been removed.</p>
                        </div>
                    </nav>

                    {/* MAIN CONTENT */}
                    <main className="flex-1 bg-slate-950 flex flex-col relative">
                        
                        {view === 'chat' && (
                            <>
                                <header className="h-20 border-b border-slate-800 flex items-center justify-between px-8 glass">
                                    <div className="flex items-center gap-4">
                                        <span className="text-3xl">{activeChar.avatar}</span>
                                        <div>
                                            <h2 className="font-bold text-lg">{activeChar.name}</h2>
                                            <p className="text-xs text-indigo-400">{activeChar.role} • {activeChar.model}</p>
                                        </div>
                                    </div>
                                </header>

                                <div className="flex-1 overflow-y-auto p-8 custom-scrollbar space-y-6">
                                    {(messages[activeChar.id] || []).length === 0 && (
                                        <div className="h-full flex flex-col items-center justify-center opacity-20">
                                            <Icons.Chat />
                                            <p className="mt-4">Start your unlimited session with {activeChar.name}</p>
                                        </div>
                                    )}
                                    {(messages[activeChar.id] || []).map((m, i) => (
                                        <div key={i} className={`flex ${m.role === 'user' ? 'justify-end' : 'justify-start'}`}>
                                            <div className={`max-w-xl p-4 rounded-2xl ${m.role === 'user' ? 'bg-indigo-600 shadow-xl' : 'bg-slate-800 border border-slate-700 text-slate-200'}`}>
                                                <p className="text-sm leading-relaxed">{m.text}</p>
                                                <span className="text-[10px] block mt-2 opacity-50">{m.time}</span>
                                            </div>
                                        </div>
                                    ))}
                                    <div ref={scrollRef} />
                                </div>

                                <div className="p-6">
                                    <div className="max-w-4xl mx-auto flex gap-4 bg-slate-900 p-2 rounded-2xl border border-slate-800 shadow-2xl">
                                        <input 
                                            value={inputText}
                                            onChange={(e) => setInputText(e.target.value)}
                                            onKeyDown={(e) => e.key === 'Enter' && sendMessage()}
                                            placeholder={`Type a message to ${activeChar.name}...`}
                                            className="flex-1 bg-transparent border-none focus:ring-0 px-4 text-sm"
                                        />
                                        <button onClick={sendMessage} className="bg-indigo-600 hover:bg-indigo-500 p-3 rounded-xl transition shadow-lg shadow-indigo-500/20">
                                            <Icons.Send />
                                        </button>
                                    </div>
                                </div>
                            </>
                        )}

                        {view === 'gallery' && (
                            <div className="p-10 overflow-y-auto h-full">
                                <h2 className="text-3xl font-bold mb-8">Character Hub</h2>
                                <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                                    {INITIAL_CHARACTERS.map(c => (
                                        <div key={c.id} onClick={() => { setActiveChar(c); setView('chat'); }} className="bg-slate-900 border border-slate-800 p-6 rounded-3xl hover:border-indigo-500 transition-all cursor-pointer group">
                                            <span className="text-5xl block mb-4 group-hover:scale-110 transition-transform">{c.avatar}</span>
                                            <h3 className="text-xl font-bold mb-1">{c.name}</h3>
                                            <p className="text-indigo-400 text-xs font-bold mb-4 uppercase tracking-widest">{c.role}</p>
                                            <p className="text-slate-400 text-sm italic">"{c.bio}"</p>
                                        </div>
                                    ))}
                                </div>
                            </div>
                        )}

                        {view === 'models' && (
                            <div className="p-10 overflow-y-auto h-full">
                                <div className="flex justify-between items-center mb-10">
                                    <div>
                                        <h2 className="text-3xl font-bold">Model Training Center</h2>
                                        <p className="text-slate-400 mt-2">Fine-tune logic and personality parameters for custom deployment.</p>
                                    </div>
                                    <button onClick={() => setIsTraining(true)} className="bg-indigo-600 px-6 py-3 rounded-xl font-bold hover:bg-indigo-500 transition flex items-center gap-2">
                                        <Icons.Cpu /> Add New Model
                                    </button>
                                </div>

                                <div className="bg-slate-900 rounded-3xl border border-slate-800 overflow-hidden">
                                    <table className="w-full text-left">
                                        <thead className="bg-slate-800/50 text-xs font-bold uppercase text-slate-500">
                                            <tr>
                                                <th className="p-6">Model ID</th>
                                                <th className="p-6">Type</th>
                                                <th className="p-6">Temp (Creativity)</th>
                                                <th className="p-6">Status</th>
                                            </tr>
                                        </thead>
                                        <tbody className="divide-y divide-slate-800">
                                            {models.map(m => (
                                                <tr key={m.id} className="hover:bg-slate-800/20">
                                                    <td className="p-6 font-mono text-indigo-400 font-bold">{m.id}</td>
                                                    <td className="p-6 text-sm">{m.type}</td>
                                                    <td className="p-6 text-sm">{m.temp}</td>
                                                    <td className="p-6">
                                                        <span className="px-3 py-1 bg-emerald-500/10 text-emerald-400 rounded-full text-[10px] font-bold border border-emerald-500/20 tracking-tighter">● {m.status}</span>
                                                    </td>
                                                </tr>
                                            ))}
                                        </tbody>
                                    </table>
                                </div>

                                {isTraining && (
                                    <div className="fixed inset-0 bg-slate-950/90 flex items-center justify-center p-6 z-50">
                                        <div className="bg-slate-900 border border-slate-700 p-8 rounded-3xl w-full max-w-md shadow-2xl">
                                            <h3 className="text-xl font-bold mb-6">Create Custom Model</h3>
                                            <div className="space-y-4">
                                                <div>
                                                    <label className="text-xs text-slate-400 block mb-2">Internal Name</label>
                                                    <input id="m_name" className="w-full bg-slate-800 border-slate-700 rounded-xl p-3 focus:ring-1 ring-indigo-500 outline-none" placeholder="e.g. Luna-Story-v2" />
                                                </div>
                                                <div>
                                                    <label className="text-xs text-slate-400 block mb-2">Base Architecture</label>
                                                    <select className="w-full bg-slate-800 border-slate-700 rounded-xl p-3 outline-none">
                                                        <option>Luna Core v1</option>
                                                        <option>Luna Logic Alpha</option>
                                                    </select>
                                                </div>
                                                <div className="pt-4 flex gap-4">
                                                    <button onClick={() => setIsTraining(false)} className="flex-1 py-3 rounded-xl hover:bg-slate-800 font-bold">Cancel</button>
                                                    <button onClick={() => {
                                                        const name = document.getElementById('m_name').value || 'New-Model';
                                                        setModels([...models, { id: name, type: 'Custom', status: 'Active', temp: 0.7 }]);
                                                        setIsTraining(false);
                                                    }} className="flex-1 py-3 bg-indigo-600 rounded-xl font-bold shadow-lg shadow-indigo-500/20">Deploy Model</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                )}
                            </div>
                        )}
                    </main>
                </div>
            );
        }

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<LunaChatApp />);
    </script>
</body>
</html>
