<h1>Hi, I'm Josie! <a href="https://www.linkedin.com/in/josieredd/">Cybersecurity Professional</a> </h1>

<h2>👨‍💻 Cybersecurity Projects:</h2>
import React from "react";
import { BrowserRouter as Router, Route, Routes, Link } from "react-router-dom";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

const Home = () => (
  <div className="text-center p-10">
    <h1 className="text-4xl font-bold">Cybersecurity Portfolio</h1>
    <p className="text-lg mt-4">Showcasing expertise in governance, risk, and compliance.</p>
    <Button className="mt-6" asChild>
      <Link to="/projects">View Projects</Link>
    </Button>
  </div>
);

const projects = [
  {
    title: "Cybersecurity Governance & Risk Management",
    description: "Developed a corporate risk management plan with BIA, risk assessments, and compliance alignment.",
  },
  {
    title: "PCI-DSS Policy Standardization",
    description: "Established a PCI-DSS governance framework, ensuring encryption and compliance with audit requirements.",
  },
  {
    title: "Data Protection & Compliance Automation",
    description: "Designed SQL-powered Power BI dashboards for compliance tracking and governance reporting.",
  },
  {
    title: "Incident Response & Security Documentation",
    description: "Authored cybersecurity playbooks and SOPs for security teams handling threats and vulnerabilities.",
  },
  {
    title: "Governance & Compliance Framework Implementation",
    description: "Developed enterprise-wide governance frameworks to enhance procedural compliance.",
  },
];

const Projects = () => (
  <div className="p-10">
    <h2 className="text-3xl font-semibold">Projects</h2>
    <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mt-6">
      {projects.map((project, index) => (
        <Card key={index}>
          <CardContent className="p-6">
            <h3 className="text-xl font-bold">{project.title}</h3>
            <p className="mt-2">{project.description}</p>
          </CardContent>
        </Card>
      ))}
    </div>
  </div>
);

const App = () => (
  <Router>
    <nav className="p-4 shadow-md flex justify-between">
      <Link to="/" className="text-lg font-bold">Home</Link>
      <Link to="/projects" className="text-lg font-bold">Projects</Link>
    </nav>
    <Routes>
      <Route path="/" element={<Home />} />
      <Route path="/projects" element={<Projects />} />
    </Routes>
  </Router>
);

export default App;
<h2> Certifications:</h2>
CompTIA Security+ CE

CompTIA CySA+

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
