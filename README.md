import Image from 'next/image'
import { Mail, Phone, MapPin, Globe, Github, Linkedin } from 'lucide-react'

export default function Resume() {
  return (
    <div className="min-h-screen bg-gray-100 py-10 px-4 sm:px-6">
      <div className="max-w-4xl mx-auto bg-white shadow-lg rounded-lg overflow-hidden">
        {/* Header Section */}
        <div className="bg-gradient-to-r from-blue-600 to-blue-800 text-white p-6 md:p-8 md:flex md:items-center">
          <div className="md:w-1/4 mb-4 md:mb-0 flex justify-center">
            <div className="relative w-32 h-32 rounded-full overflow-hidden border-4 border-white">
              <Image 
                src="/placeholder.svg?height=128&width=128" 
                alt="Profile" 
                width={128} 
                height={128} 
                className="object-cover"
              />
            </div>
          </div>
          <div className="md:w-3/4 md:pl-6">
            <h1 className="text-3xl font-bold mb-1">John Doe</h1>
            <h2 className="text-xl text-blue-100 mb-4">Senior Frontend Developer</h2>
            <div className="grid grid-cols-1 md:grid-cols-2 gap-2 text-sm">
              <div className="flex items-center">
                <Mail className="h-4 w-4 mr-2" />
                <span>john.doe@example.com</span>
              </div>
              <div className="flex items-center">
                <Phone className="h-4 w-4 mr-2" />
                <span>(123) 456-7890</span>
              </div>
              <div className="flex items-center">
                <MapPin className="h-4 w-4 mr-2" />
                <span>San Francisco, CA</span>
              </div>
              <div className="flex items-center">
                <Globe className="h-4 w-4 mr-2" />
                <span>johndoe.com</span>
              </div>
              <div className="flex items-center">
                <Github className="h-4 w-4 mr-2" />
                <span>github.com/johndoe</span>
              </div>
              <div className="flex items-center">
                <Linkedin className="h-4 w-4 mr-2" />
                <span>linkedin.com/in/johndoe</span>
              </div>
            </div>
          </div>
        </div>

        {/* Main Content */}
        <div className="p-6 md:p-8">
          {/* Professional Summary */}
          <section className="mb-8">
            <h3 className="text-xl font-bold text-gray-800 border-b-2 border-blue-600 pb-2 mb-4">
              Professional Summary
            </h3>
            <p className="text-gray-700 leading-relaxed">
              Passionate and detail-oriented Frontend Developer with 8+ years of experience creating responsive, 
              user-friendly web applications. Proficient in React, Next.js, and modern JavaScript. Strong 
              background in UI/UX principles and performance optimization. Committed to writing clean, maintainable 
              code and staying current with emerging technologies and best practices.
            </p>
          </section>

          {/* Work Experience */}
          <section className="mb-8">
            <h3 className="text-xl font-bold text-gray-800 border-b-2 border-blue-600 pb-2 mb-4">
              Work Experience
            </h3>
            
            <div className="mb-6">
              <div className="flex flex-wrap justify-between items-start mb-2">
                <h4 className="text-lg font-semibold text-gray-800">Senior Frontend Developer</h4>
                <div className="text-sm text-gray-600 font-medium">Jan 2020 - Present</div>
              </div>
              <div className="text-md font-medium text-blue-600 mb-2">TechCorp Inc., San Francisco, CA</div>
              <ul className="list-disc list-inside text-gray-700 space-y-1">
                <li>Led the frontend development of the company's flagship SaaS product, improving user engagement by 35%</li>
                <li>Architected and implemented a component library used across multiple products</li>
                <li>Mentored junior developers and conducted code reviews to ensure quality standards</li>
                <li>Optimized application performance, reducing load times by 40%</li>
              </ul>
            </div>

            <div className="mb-6">
              <div className="flex flex-wrap justify-between items-start mb-2">
                <h4 className="text-lg font-semibold text-gray-800">Frontend Developer</h4>
                <div className="text-sm text-gray-600 font-medium">Mar 2017 - Dec 2019</div>
              </div>
              <div className="text-md font-medium text-blue-600 mb-2">WebSolutions LLC, Austin, TX</div>
              <ul className="list-disc list-inside text-gray-700 space-y-1">
                <li>Developed responsive web applications for clients across various industries</li>
                <li>Collaborated with designers to implement pixel-perfect UI components</li>
                <li>Integrated RESTful APIs and implemented state management solutions</li>
                <li>Participated in agile development processes and sprint planning</li>
              </ul>
            </div>

            <div>
              <div className="flex flex-wrap justify-between items-start mb-2">
                <h4 className="text-lg font-semibold text-gray-800">Junior Web Developer</h4>
                <div className="text-sm text-gray-600 font-medium">Jun 2015 - Feb 2017</div>
              </div>
              <div className="text-md font-medium text-blue-600 mb-2">Digital Creations, Portland, OR</div>
              <ul className="list-disc list-inside text-gray-700 space-y-1">
                <li>Built and maintained client websites using HTML, CSS, and JavaScript</li>
                <li>Assisted senior developers with larger projects and bug fixes</li>
                <li>Created responsive email templates and marketing materials</li>
              </ul>
            </div>
          </section>

          {/* Education */}
          <section className="mb-8">
            <h3 className="text-xl font-bold text-gray-800 border-b-2 border-blue-600 pb-2 mb-4">
              Education
            </h3>
            
            <div className="mb-4">
              <div className="flex flex-wrap justify-between items-start">
                <h4 className="text-lg font-semibold text-gray-800">Bachelor of Science in Computer Science</h4>
                <div className="text-sm text-gray-600 font-medium">2011 - 2015</div>
              </div>
              <div className="text-md font-medium text-blue-600">University of California, Berkeley</div>
              <p className="text-gray-700 mt-1">GPA: 3.8/4.0 - Dean's List</p>
            </div>
          </section>

          {/* Skills */}
          <section className="mb-8">
            <h3 className="text-xl font-bold text-gray-800 border-b-2 border-blue-600 pb-2 mb-4">
              Skills
            </h3>
            
            <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
              <div>
                <h4 className="text-lg font-semibold text-gray-800 mb-2">Technical Skills</h4>
                <div className="flex flex-wrap gap-2">
                  {['JavaScript', 'TypeScript', 'React', 'Next.js', 'HTML5', 'CSS3', 'Tailwind CSS', 'Redux', 'GraphQL', 'REST APIs', 'Git', 'Webpack'].map((skill) => (
                    <span key={skill} className="bg-blue-100 text-blue-800 text-sm font-medium px-3 py-1 rounded-full">
                      {skill}
                    </span>
                  ))}
                </div>
              </div>
              
              <div>
                <h4 className="text-lg font-semibold text-gray-800 mb-2">Soft Skills</h4>
                <div className="flex flex-wrap gap-2">
                  {['Team Leadership', 'Project Management', 'Problem Solving', 'Communication', 'Mentoring', 'Agile Methodologies'].map((skill) => (
                    <span key={skill} className="bg-green-100 text-green-800 text-sm font-medium px-3 py-1 rounded-full">
                      {skill}
                    </span>
                  ))}
                </div>
              </div>
            </div>
          </section>

          {/* Projects */}
          <section className="mb-8">
            <h3 className="text-xl font-bold text-gray-800 border-b-2 border-blue-600 pb-2 mb-4">
              Projects
            </h3>
            
            <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
              <div className="border border-gray-200 rounded-lg p-4 hover:shadow-md transition-shadow">
                <h4 className="text-lg font-semibold text-gray-800 mb-1">E-commerce Platform</h4>
                <p className="text-sm text-gray-600 mb-2">React, Next.js, Stripe, MongoDB</p>
                <p className="text-gray-700 text-sm">
                  Developed a full-featured e-commerce platform with secure payment processing, 
                  inventory management, and an admin dashboard.
                </p>
              </div>
              
              <div className="border border-gray-200 rounded-lg p-4 hover:shadow-md transition-shadow">
                <h4 className="text-lg font-semibold text-gray-800 mb-1">Task Management App</h4>
                <p className="text-sm text-gray-600 mb-2">React, Redux, Firebase</p>
                <p className="text-gray-700 text-sm">
                  Built a collaborative task management application with real-time updates, 
                  user authentication, and team workspaces.
                </p>
              </div>
              
              <div className="border border-gray-200 rounded-lg p-4 hover:shadow-md transition-shadow">
                <h4 className="text-lg font-semibold text-gray-800 mb-1">Weather Dashboard</h4>
                <p className="text-sm text-gray-600 mb-2">JavaScript, OpenWeather API, Chart.js</p>
                <p className="text-gray-700 text-sm">
                  Created an interactive weather dashboard with location-based forecasts, 
                  historical data visualization, and severe weather alerts.
                </p>
              </div>
              
              <div className="border border-gray-200 rounded-lg p-4 hover:shadow-md transition-shadow">
                <h4 className="text-lg font-semibold text-gray-800 mb-1">Portfolio Website</h4>
                <p className="text-sm text-gray-600 mb-2">Next.js, Tailwind CSS, Framer Motion</p>
                <p className="text-gray-700 text-sm">
                  Designed and developed a personal portfolio website with smooth animations, 
                  responsive design, and optimized performance.
                </p>
              </div>
            </div>
          </section>

          {/* Certifications */}
          <section>
            <h3 className="text-xl font-bold text-gray-800 border-b-2 border-blue-600 pb-2 mb-4">
              Certifications
            </h3>
            
            <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
              <div className="flex items-start">
                <div className="bg-blue-100 p-2 rounded-md mr-3">
                  <svg className="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
                  </svg>
                </div>
                <div>
                  <h4 className="text-md font-semibold text-gray-800">AWS Certified Developer</h4>
                  <p className="text-sm text-gray-600">Amazon Web Services, 2022</p>
                </div>
              </div>
              
              <div className="flex items-start">
                <div className="bg-blue-100 p-2 rounded-md mr-3">
                  <svg className="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
                  </svg>
                </div>
                <div>
                  <h4 className="text-md font-semibold text-gray-800">Google UX Design Professional Certificate</h4>
                  <p className="text-sm text-gray-600">Google, 2021</p>
                </div>
              </div>
              
              <div className="flex items-start">
                <div className="bg-blue-100 p-2 rounded-md mr-3">
                  <svg className="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
                  </svg>
                </div>
                <div>
                  <h4 className="text-md font-semibold text-gray-800">React Advanced Concepts</h4>
                  <p className="text-sm text-gray-600">Frontend Masters, 2020</p>
                </div>
              </div>
              
              <div className="flex items-start">
                <div className="bg-blue-100 p-2 rounded-md mr-3">
                  <svg className="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
                  </svg>
                </div>
                <div>
                  <h4 className="text-md font-semibold text-gray-800">Certified Scrum Master</h4>
                  <p className="text-sm text-gray-600">Scrum Alliance, 2019</p>
                </div>
              </div>
            </div>
          </section>
        </div>

        {/* Footer */}
        <div className="bg-gray-50 px-6 py-4 text-center text-sm text-gray-600 border-t">
          <p>References available upon request</p>
        </div>
      </div>
    </div>
  )
}
