import React from "react";
import { Linkedin, Mail, Terminal, Cpu, Code2, Globe } from "lucide-react";

export default function GitHubProfile() {
  const profileData = {
    name: "Dikshika Adhikari",
    role: "IT Student & Aspiring Full Stack Developer",
    coreFocus: ["MERN Stack", "Next.js", "TypeScript", "AI Integrations"],
    toolset: ["AntiGravity", "Codex"],
    currentQuest: "Building intelligent, scalable web applications with modern AI tooling",
  };

  const stack = {
    languages: ["TypeScript", "JavaScript (ES6+)", "HTML5", "CSS3"],
    frameworks: ["Next.js", "React.js", "Express.js", "Tailwind CSS"],
    backend: ["Node.js", "MongoDB"],
    aiTooling: ["Codex", "OpenAI API", "Gemini API", "Prompt Engineering"],
    workflow: ["AntiGravity", "Git", "GitHub", "VS Code", "Postman"],
  };

  return (
    <div className="min-h-screen bg-slate-950 text-slate-100 p-4 md:p-12 relative overflow-hidden font-sans">
      {/* Background Radial Glow Effect */}
      <div className="absolute top-0 left-1/4 w-96 h-96 bg-purple-600/20 rounded-full blur-3xl pointer-events-none" />
      <div className="absolute bottom-0 right-1/4 w-96 h-96 bg-blue-600/20 rounded-full blur-3xl pointer-events-none" />

      <div className="max-w-4xl mx-auto space-y-8 relative z-10">
        {/* HEADER SECTION */}
        <header className="text-center space-y-4 border-b border-slate-800 pb-8">
          <h1 className="text-4xl md:text-5xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-purple-400 to-blue-400">
            ⚡ Hi, I'm {profileData.name}
          </h1>
          <p className="text-sm md:text-base font-semibold text-purple-400 tracking-wider uppercase">
            Full Stack Engineer in Training • MERN + Next.js + AI Integrations
          </p>

          <div className="flex justify-center gap-4 pt-2">
            <a
              href="https://www.linkedin.com/in/dikshika-adhikari-66857b411/"
              target="_blank"
              rel="noreferrer"
              className="flex items-center gap-2 bg-blue-600 hover:bg-blue-700 text-white px-4 py-2 rounded-lg font-medium text-sm transition"
            >
              <Linkedin className="w-4 h-4" /> LinkedIn
            </a>
            <a
              href="mailto:deekshikaadhikari@gmail.com"
              className="flex items-center gap-2 bg-red-600 hover:bg-red-700 text-white px-4 py-2 rounded-lg font-medium text-sm transition"
            >
              <Mail className="w-4 h-4" /> Email
            </a>
          </div>
        </header>

        {/* DEVELOPER INTERFACE OBJECT */}
        <section className="bg-slate-900/80 border border-slate-800 rounded-xl p-5 font-mono text-sm shadow-xl">
          <div className="flex items-center gap-2 text-slate-500 mb-3 border-b border-slate-800 pb-2">
            <Code2 className="w-4 h-4 text-purple-400" /> developer.ts
          </div>
          <pre className="text-blue-300 overflow-x-auto">
            <code>
              <span className="text-pink-400">interface</span> Developer &#123;{"\n"}
              {"  "}name: <span className="text-teal-300">string</span>;{"\n"}
              {"  "}role: <span class="text-teal-300">string</span>;{"\n"}
              {"  "}coreFocus: <span className="text-teal-300">string[]</span>;{"\n"}
              {"  "}toolset: <span className="text-teal-300">string[]</span>;{"\n"}
              {"  "}currentQuest: <span className="text-teal-300">string</span>;{"\n"}
              &#125;{"\n\n"}
              <span className="text-pink-400">const</span> dikshika: Developer = {JSON.stringify(profileData, null, 2)}
            </code>
          </pre>
        </section>

        {/* DEVELOPMENT PIPELINE */}
        <section className="space-y-4">
          <h2 className="text-xl font-bold flex items-center gap-2 text-slate-200">
            <Cpu className="w-5 h-5 text-purple-400" /> Development Path
          </h2>
          <div className="grid grid-cols-1 md:grid-cols-3 gap-4">
            <div className="bg-slate-900 border border-emerald-500/30 rounded-lg p-4">
              <h3 className="text-emerald-400 font-bold mb-2">✔ Complete</h3>
              <ul className="text-xs text-slate-400 space-y-1 list-disc list-inside">
                <li>HTML5 / CSS3</li>
                <li>Modern JavaScript</li>
                <li>Git & Version Control</li>
              </ul>
            </div>
            <div className="bg-slate-900 border border-amber-500/30 rounded-lg p-4">
              <h3 className="text-amber-400 font-bold mb-2">⚡ In Progress</h3>
              <ul className="text-xs text-slate-400 space-y-1 list-disc list-inside">
                <li>TypeScript & Next.js</li>
                <li>Node.js & MongoDB</li>
                <li>AntiGravity & Codex</li>
              </ul>
            </div>
            <div className="bg-slate-900 border border-pink-500/30 rounded-lg p-4">
              <h3 className="text-pink-400 font-bold mb-2">🎯 Target</h3>
              <ul className="text-xs text-slate-400 space-y-1 list-disc list-inside">
                <li>AI Agent Workflows</li>
                <li>Full-Stack AI Apps</li>
                <li>Production Deployments</li>
              </ul>
            </div>
          </div>
        </section>

        {/* CORE TECH STACK */}
        <section className="bg-slate-900/80 border border-slate-800 rounded-xl p-5 font-mono text-sm">
          <h2 className="text-lg font-bold text-slate-200 mb-3 flex items-center gap-2">
            <Globe className="w-5 h-5 text-blue-400" /> Core Tech Stack
          </h2>
          <pre className="text-amber-300 overflow-x-auto">
            <code>
              <span className="text-pink-400">const</span> stack = {JSON.stringify(stack, null, 2)}
            </code>
          </pre>
        </section>

        {/* SYSTEM TERMINAL */}
        <section className="bg-black border border-slate-800 rounded-xl p-5 font-mono text-xs text-emerald-400 space-y-3">
          <div className="flex items-center gap-2 text-slate-500 border-b border-slate-900 pb-2">
            <Terminal className="w-4 h-4 text-emerald-400" /> bash
          </div>
          <div>
            <p className="text-slate-500"># Current Status</p>
            <p className="text-slate-200">$ dikshika --status</p>
            <p className="text-emerald-400">&gt; Leveling up MERN, Next.js, and TypeScript with hands-on AI integration using Codex & AntiGravity.</p>
          </div>
          <div>
            <p className="text-slate-500"># Goals</p>
            <p className="text-slate-200">$ dikshika --goals</p>
            <p className="text-emerald-400">&gt; 1. Build & deploy 3 production-ready AI-powered web apps.</p>
            <p className="text-emerald-400">&gt; 2. Master full-stack state management and serverless APIs.</p>
          </div>
        </section>

        {/* FOOTER */}
        <footer className="text-center text-xs text-slate-500 border-t border-slate-800 pt-6">
          Designed & Developed by <span className="text-slate-300 font-semibold">{profileData.name}</span>
        </footer>
      </div>
    </div>
  );
}
