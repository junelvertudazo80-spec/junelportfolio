import { motion } from "framer-motion";
import { Mail, Phone, Linkedin, Award, Target } from "lucide-react";

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-gray-900 via-gray-800 to-black text-white font-sans">
      {/* Hero Section */}
      <section className="flex flex-col items-center justify-center text-center py-20 px-6">
        <motion.h1
          initial={{ opacity: 0, y: -50 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 1 }}
          className="text-5xl md:text-6xl font-bold mb-4 bg-clip-text text-transparent bg-gradient-to-r from-pink-500 to-purple-400"
        >
          Junel Vertudazo
        </motion.h1>
        <p className="text-lg md:text-xl text-gray-300 max-w-2xl">
          Customer Service & Sales Specialist • Team Leader • Performance Coach
        </p>
      </section>

      {/* About Section */}
      <section className="max-w-5xl mx-auto px-6 py-16 grid md:grid-cols-2 gap-10 items-center">
        <motion.img
          whileHover={{ scale: 1.05 }}
          src="/profile.jpg"
          alt="Junel Vertudazo"
          className="rounded-2xl shadow-lg border border-gray-700"
        />
        <div>
          <h2 className="text-3xl font-bold mb-4">About Me</h2>
          <p className="text-gray-300 mb-4">
            I’ve spent nearly a decade in the customer service industry, growing from
            frontline roles into leadership positions. Along the way, I’ve mastered conflict
            resolution, coaching, and customer experience management. While at Metro by
            T-Mobile, I successfully <span className="font-semibold text-pink-400">sold 300+ phones</span>,
            proving that I can not only support customers but also drive sales.
          </p>
          <p className="text-gray-300">
            My approach blends empathy, adaptability, and results-driven performance.
            I thrive in high-pressure environments and am always eager to embrace new
            challenges and opportunities.
          </p>
        </div>
      </section>

      {/* Skills Section */}
      <section className="bg-gray-800 py-16 px-6">
        <h2 className="text-center text-3xl font-bold mb-10">Core Skills</h2>
        <div className="grid md:grid-cols-3 gap-8 max-w-5xl mx-auto">
          <div className="p-6 rounded-2xl bg-gray-900 shadow-md hover:shadow-pink-500/30">
            <h3 className="text-xl font-semibold mb-3">Customer Experience</h3>
            <p className="text-gray-300 text-sm">
              Phone, Email & Chat Support • Conflict Resolution • Quality Assurance • Escalation Handling
            </p>
          </div>
          <div className="p-6 rounded-2xl bg-gray-900 shadow-md hover:shadow-purple-500/30">
            <h3 className="text-xl font-semibold mb-3">Leadership</h3>
            <p className="text-gray-300 text-sm">
              Team Supervision • Coaching & Mentoring • Training & Development • Performance Reviews
            </p>
          </div>
          <div className="p-6 rounded-2xl bg-gray-900 shadow-md hover:shadow-pink-400/30">
            <h3 className="text-xl font-semibold mb-3">Sales Talent</h3>
            <p className="text-gray-300 text-sm">
              Sold 300+ Phones at Metro by T-Mobile • Upselling • Customer Engagement • Loyalty Building
            </p>
          </div>
        </div>
      </section>

      {/* Achievements */}
      <section className="max-w-5xl mx-auto py-16 px-6">
        <h2 className="text-3xl font-bold text-center mb-10">Achievements</h2>
        <div className="grid md:grid-cols-2 gap-6">
          <div className="flex items-start gap-4 p-6 bg-gray-800 rounded-2xl shadow">
            <Award className="text-pink-400 w-8 h-8" />
            <p className="text-gray-300">CEO Recognize Award – 2024</p>
          </div>
          <div className="flex items-start gap-4 p-6 bg-gray-800 rounded-2xl shadow">
            <Target className="text-purple-400 w-8 h-8" />
            <p className="text-gray-300">Top Supervisor Award (Multiple Quarters)</p>
          </div>
          <div className="flex items-start gap-4 p-6 bg-gray-800 rounded-2xl shadow">
            <Award className="text-pink-400 w-8 h-8" />
            <p className="text-gray-300">Top Agent Award – Metro by T-Mobile (2022)</p>
          </div>
          <div className="flex items-start gap-4 p-6 bg-gray-800 rounded-2xl shadow">
            <Target className="text-purple-400 w-8 h-8" />
            <p className="text-gray-300">Improved FCR by 20% with coaching initiatives</p>
          </div>
        </div>
      </section>

      {/* Contact Section */}
      <section className="bg-gray-900 py-16 px-6 text-center">
        <h2 className="text-3xl font-bold mb-6">Let’s Work Together</h2>
        <p className="text-gray-400 mb-6 max-w-xl mx-auto">
          I’m always open to new opportunities where I can contribute my customer
          service expertise, leadership skills, and proven sales talent.
        </p>
        <div className="flex justify-center gap-6">
          <a href="mailto:junelvertudazo80@gmail.com" className="hover:text-pink-400">
            <Mail className="w-7 h-7" />
          </a>
          <a href="tel:+639694788523" className="hover:text-purple-400">
            <Phone className="w-7 h-7" />
          </a>
          <a href="https://www.linkedin.com/in/junel-vertudazo" className="hover:text-pink-400">
            <Linkedin className="w-7 h-7" />
          </a>
        </div>
      </section>

      {/* Footer */}
      <footer className="text-center text-gray-500 text-sm py-6 border-t border-gray-700">
        © {new Date().getFullYear()} Junel Vertudazo. All Rights Reserved.
      </footer>
    </div>
  );
}
