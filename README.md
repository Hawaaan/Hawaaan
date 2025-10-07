import { Github, Linkedin, Mail, Globe } from "lucide-react";
import { Button } from "@/components/ui/button";

const Hero = () => {
  return (
    <section className="min-h-screen flex items-center justify-center px-4 py-20">
      <div className="max-w-4xl w-full text-center space-y-8 animate-fade-in">
        {/* Animated Greeting */}
        <div className="space-y-4">
          <h1 className="text-5xl md:text-7xl font-bold">
            Hi, I'm <span className="gradient-text">Hawaaan</span> 👋
          </h1>
          <div className="text-2xl md:text-3xl text-muted-foreground space-y-2">
            <p className="animate-slide-in" style={{ animationDelay: "0.2s" }}>
              Front‑End Developer
            </p>
            <p className="text-lg md:text-xl text-primary animate-slide-in" style={{ animationDelay: "0.4s" }}>
              Clean UI • Accessible Design • Fast Apps
            </p>
          </div>
        </div>


        <p className="text-lg text-muted-foreground animate-fade-in" style={{ animationDelay: "0.6s" }}>
          💻 Front‑End Developer • 🌍 Somalia
        </p>

        {/* CTA Buttons */}
        <div className="flex flex-wrap gap-4 justify-center animate-fade-in" style={{ animationDelay: "0.8s" }}>
          <Button size="lg" className="gap-2 animate-glow-pulse">
            <Github className="h-5 w-5" />
            View Projects
          </Button>
          <Button size="lg" variant="secondary" className="gap-2">
            <Mail className="h-5 w-5" />
            Get In Touch
          </Button>
        </div>

        {/* Quick Links */}
        <div className="flex gap-4 justify-center pt-8 animate-fade-in" style={{ animationDelay: "1s" }}>
          <a href="https://github.com/Hawaaan" target="_blank" rel="noopener noreferrer" 
             className="p-3 glass-card rounded-lg hover-lift">
            <Github className="h-6 w-6" />
          </a>
          <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer"
             className="p-3 glass-card rounded-lg hover-lift">
            <Linkedin className="h-6 w-6" />
          </a>
          <a href="mailto:your@email.com"
             className="p-3 glass-card rounded-lg hover-lift">
            <Mail className="h-6 w-6" />
          </a>
          <a href="https://yoursite.com" target="_blank" rel="noopener noreferrer"
             className="p-3 glass-card rounded-lg hover-lift">
            <Globe className="h-6 w-6" />
          </a>
        </div>
      </div>
    </section>
  );
};

const About = () => {
  return (
    <section className="py-20 px-4">
      <div className="max-w-4xl mx-auto">
        <h2 className="text-4xl font-bold mb-8 text-center gradient-text">
          🧠 About Me
        </h2>
        
        <div className="glass-card p-8 rounded-2xl space-y-6">
          <p className="text-lg text-foreground/90 leading-relaxed">
            I build fast, responsive, and accessible web interfaces with modern front‑end stacks.
          </p>
          
          <div className="space-y-4">
            <div className="flex items-start gap-3">
              <span className="text-2xl">🎯</span>
              <div>
                <strong className="text-primary">Focus:</strong>
                <span className="text-muted-foreground ml-2">
                  React / Next.js, reusable components, and pixel‑perfect UI
                </span>
              </div>
            </div>
            
            <div className="flex items-start gap-3">
              <span className="text-2xl">🧩</span>
              <div>
                <strong className="text-primary">Strengths:</strong>
                <span className="text-muted-foreground ml-2">
                  Clean CSS architecture, design systems, and performance
                </span>
              </div>
            </div>
            
            <div className="flex items-start gap-3">
              <span className="text-2xl">🌱</span>
              <div>
                <strong className="text-primary">Currently:</strong>
                <span className="text-muted-foreground ml-2">
                  Deepening TypeScript & testing (Jest/RTL)
                </span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  );
};

const TechStack = () => {
  const technologies = [
    { name: "React", icon: "⚛️", color: "from-blue-400 to-cyan-400" },
    { name: "Next.js", icon: "▲", color: "from-gray-400 to-gray-600" },
    { name: "TypeScript", icon: "TS", color: "from-blue-500 to-blue-700" },
    { name: "JavaScript", icon: "JS", color: "from-yellow-400 to-yellow-600" },
    { name: "HTML5", icon: "HTML", color: "from-orange-500 to-red-500" },
    { name: "CSS3", icon: "CSS", color: "from-blue-500 to-purple-500" },
    { name: "Tailwind", icon: "🎨", color: "from-cyan-400 to-blue-500" },
    { name: "Redux", icon: "🔄", color: "from-purple-500 to-purple-700" },
    { name: "Vite", icon: "⚡", color: "from-purple-400 to-yellow-400" },
    { name: "Git", icon: "📦", color: "from-orange-600 to-red-600" },
    { name: "Figma", icon: "🎯", color: "from-pink-500 to-purple-500" },
    { name: "Vercel", icon: "▼", color: "from-gray-700 to-black" },
  ];

  return (
    <section className="py-20 px-4 bg-secondary/20">
      <div className="max-w-6xl mx-auto">
        <h2 className="text-4xl font-bold mb-12 text-center gradient-text">
          🧰 Tech Stack
        </h2>
        
        <div className="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
          {technologies.map((tech, index) => (
            <div
              key={tech.name}
              className="glass-card p-6 rounded-xl text-center hover-lift group"
              style={{ animationDelay: `${index * 0.1}s` }}
            >
              <div className={`text-5xl mb-3 bg-gradient-to-br ${tech.color} bg-clip-text text-transparent group-hover:scale-110 transition-transform duration-300`}>
                {tech.icon}
              </div>
              <h3 className="font-semibold text-foreground">{tech.name}</h3>
            </div>
          ))}
        </div>
        
        <p className="text-center text-muted-foreground mt-8 text-sm">
          ✨ Minimal design • Fast performance • Accessible by default ✨
        </p>
      </div>
    </section>
  );
};

const Experience = () => {
  return (
    <section className="py-20 px-4">
      <div className="max-w-4xl mx-auto">
        <h2 className="text-4xl font-bold mb-12 text-center gradient-text">
          💼 Experience & Education
        </h2>
        
        <div className="space-y-8">
          {/* Freelance Experience */}
          <div className="glass-card p-8 rounded-2xl hover-lift">
            <div className="flex flex-col md:flex-row md:items-center md:justify-between mb-4">
              <h3 className="text-2xl font-bold text-foreground">Front‑End Developer</h3>
              <span className="text-muted-foreground">2021–Present</span>
            </div>
            <p className="text-primary font-semibold mb-4">Freelance</p>
            <ul className="space-y-3 text-muted-foreground">
              <li className="flex items-start gap-2">
                <span className="text-primary mt-1">▹</span>
                <span>Built responsive UIs and design systems; shipped sites on Vercel/Netlify</span>
              </li>
              <li className="flex items-start gap-2">
                <span className="text-primary mt-1">▹</span>
                <span>Improved performance (Lighthouse 90+) with code‑splitting and image optimization</span>
              </li>
            </ul>
          </div>

          {/* Education */}
          <div className="glass-card p-8 rounded-2xl hover-lift">
            <h3 className="text-2xl font-bold text-foreground mb-4">Education</h3>
            <p className="text-primary font-semibold mb-4">Self‑taught + courses</p>
            <div className="flex flex-wrap gap-2">
              {["React", "Next.js", "TailwindCSS", "TypeScript"].map((skill) => (
                <span
                  key={skill}
                  className="px-4 py-2 bg-primary/10 border border-primary/20 rounded-full text-sm text-primary"
                >
                  {skill}
                </span>
              ))}
            </div>
          </div>
        </div>
      </div>
    </section>
  );
};

const Footer = () => {
  return (
    <footer className="py-12 px-4 border-t border-border/50">
      <div className="max-w-4xl mx-auto text-center space-y-6">
        <h2 className="text-3xl font-bold gradient-text">
          🌐 Let's Connect
        </h2>
        
        <div className="flex flex-wrap justify-center gap-4">
          <a
            href="mailto:your@email.com"
            className="px-6 py-3 glass-card rounded-lg hover-lift text-sm font-medium"
          >
            📧 Email
          </a>
          <a
            href="https://linkedin.com"
            target="_blank"
            rel="noopener noreferrer"
            className="px-6 py-3 glass-card rounded-lg hover-lift text-sm font-medium"
          >
            💼 LinkedIn
          </a>
          <a
            href="https://twitter.com"
            target="_blank"
            rel="noopener noreferrer"
            className="px-6 py-3 glass-card rounded-lg hover-lift text-sm font-medium"
          >
            🐦 Twitter
          </a>
          <a
            href="https://yoursite.com"
            target="_blank"
            rel="noopener noreferrer"
            className="px-6 py-3 glass-card rounded-lg hover-lift text-sm font-medium"
          >
            🌐 Portfolio
          </a>
        </div>

        <div className="pt-8 text-muted-foreground">
          <p className="text-xl font-semibold mb-2">
            ✨ "Design it simple. Build it fast. Make it accessible." ✨
          </p>
          <p className="text-sm">
            © 2025 Hawaaan • Built with React & TailwindCSS
          </p>
        </div>
      </div>
    </footer>
  );
};

const Index = () => {
  return (
    <div className="min-h-screen">
      <Hero />
      <About />
      <TechStack />
      <Experience />
      <Footer />
    </div>
  );
};

export default Index;
