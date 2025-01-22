# ResumeDesignWithFigmaClaude
This project was assigned in our Innovative Technologies class at the University of Colorado CMCI Department
The brief was to sketch out and create 3 different Figma templates for our resume
Then pull the Figma template into Claude.ai to create a website, including code

I have a lot to learn about coding and GitHub, so here's the start!

Figma Files Below, including icons I made with Adobe Illustrator
![Desktop - 4](https://github.com/user-attachments/assets/88a90072-5e39-4f3b-8de9-d8ac6358e3a8)
![Desktop - 3](https://github.com/user-attachments/assets/8f69de33-a227-4249-b633-3cfbe912e0cb)
![Desktop - 2](https://github.com/user-attachments/assets/2aeb8c45-94f5-4759-a691-1aabef46448b)

I wanted to start with the basics, so my prompt to Claude.ai reflects this:
"Please help me turn this Figma esign into a website" (yes, I use manners with AI bots, just incase ;) )

This recording shows the formatting Claude.ai provided, with space to add the images:
https://github.com/user-attachments/assets/1386bce6-b3e4-42e2-a7a4-36a2e62fb274

https://github.com/user-attachments/assets/f9b41f9d-bf2c-4c08-b406-a8872d8ba4f9


The following is the code provided by Claude.ai:

import React from 'react';
import { Card } from '@/components/ui/card';

const Portfolio = () => {
  const education = [
    {
      degree: "Masters in Strategic Communication Design",
      school: "University of Colorado Boulder",
      years: "2024-Present"
    },
    {
      degree: "B.A. Interdisciplinary - Communication & Somatic Psychology",
      school: "Naropa University",
      years: "2022-2023"
    },
    {
      degree: "Associate of Arts and Sciences",
      school: "Minnesota State Community & Technical College",
      years: "2015-2018"
    }
  ];

  const coreCompetencies = [
    "Podcast Production & Management",
    "Social Media Strategy",
    "Visual Content Creation",
    "Brand Development",
    "Copywriting & Show Notes",
    "Team Collaboration",
    "Project Management",
    "Community Engagement"
  ];

  const technicalSkills = [
    "Podcast Production: Garage Band, BuzzSprout, Fireside, Audioboom",
    "Design Software: Canva, Figma, Adobe Creative Suite",
    "Content Management: Amplify, Meta Suite, HootSuite, Later, Planoly",
    "Web Development: WordPress, Squarespace, Wix",
    "Digital Marketing: SEO, Social Media Analytics, Content Calendar Management",
    "Languages: English (Native), Spanish (In Progress)"
  ];

  return (
    <div className="min-h-screen bg-gray-100 p-8">
      <div className="max-w-4xl mx-auto">
        {/* Header Section */}
        <div className="bg-white rounded-lg shadow-lg p-8 mb-8">
          <div className="flex flex-col md:flex-row items-center gap-8">
            <div className="w-48 h-48 rounded-full overflow-hidden bg-gray-200">
              <img 
                src="/api/placeholder/192/192" 
                alt="Profile" 
                className="w-full h-full object-cover"
              />
            </div>
            <div>
              <h1 className="text-3xl font-bold mb-2">Alexandra Susann Frederick</h1>
              <h2 className="text-xl text-gray-600 mb-4">Designer, Brand Builder, Podcast Strategist</h2>
              <p className="text-gray-700">
                Versatile digital content creator with 7+ years of experience in podcast production,
                social media management, and design. Demonstrated success in growing audience
                engagement, managing multi-platform content strategies, and creating compelling
                visual assets.
              </p>
            </div>
          </div>
        </div>

        {/* Portfolio Grid */}
        <div className="grid grid-cols-2 md:grid-cols-5 gap-4 mb-8">
          {[1, 2, 3, 4, 5].map((item) => (
            <div key={item} className="aspect-square bg-gray-200 rounded-lg overflow-hidden">
              <img 
                src={`/api/placeholder/200/200`} 
                alt={`Portfolio item ${item}`}
                className="w-full h-full object-cover"
              />
            </div>
          ))}
        </div>

        {/* Main Content Grid */}
        <div className="grid md:grid-cols-2 gap-8">
          {/* Left Column */}
          <div className="space-y-8">
            <Card className="p-6">
              <h2 className="text-xl font-bold mb-4">Education</h2>
              <div className="space-y-4">
                {education.map((edu, index) => (
                  <div key={index}>
                    <h3 className="font-semibold">{edu.degree}</h3>
                    <p className="text-gray-600">{edu.school}</p>
                    <p className="text-gray-500 text-sm">{edu.years}</p>
                  </div>
                ))}
              </div>
            </Card>

            <Card className="p-6">
              <h2 className="text-xl font-bold mb-4">Core Competencies</h2>
              <ul className="space-y-2">
                {coreCompetencies.map((skill, index) => (
                  <li key={index} className="flex items-center gap-2">
                    <div className="w-2 h-2 bg-blue-500 rounded-full"></div>
                    {skill}
                  </li>
                ))}
              </ul>
            </Card>
          </div>

          {/* Right Column */}
          <div className="space-y-8">
            <Card className="p-6">
              <h2 className="text-xl font-bold mb-4">Technical Skills</h2>
              <ul className="space-y-3">
                {technicalSkills.map((skill, index) => (
                  <li key={index} className="text-gray-700">{skill}</li>
                ))}
              </ul>
            </Card>

            <Card className="p-6">
              <h2 className="text-xl font-bold mb-4">Experience Highlights</h2>
              <div className="space-y-4">
                <div>
                  <h3 className="font-semibold">PODCAST PRODUCER & DIGITAL CONTENT MANAGER</h3>
                  <p className="text-gray-600">Naropa University | 2021-2023</p>
                  <ul className="mt-2 space-y-2 text-gray-700">
                    <li>• Managed Mindful U Podcast content, growing listenership to 303K+ downloads</li>
                    <li>• Coordinated integrated promotional campaigns across platforms</li>
                    <li>• Managed social media presence with 12.3K Instagram and 45.6K Facebook followers</li>
                  </ul>
                </div>
              </div>
            </Card>
          </div>
        </div>
      </div>
    </div>
  );
};

export default Portfolio;

I lack the current coding language to know what is going on here enough to read or edit this yet, but with more practice I will continue to learn!
I lean towards optimism - and even though learning something new can be intimidating (often frustrating!), I am excited to see the progress that happens in Innovative Tech class this semester.
