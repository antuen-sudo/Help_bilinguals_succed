# Help_bilinguals_succed
Helping Bilingual seellers get ahead in the corporate sales enviroenment 
import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Mail, Users, Zap, MapPin } from "lucide-react";
import { motion } from "framer-motion";

// Single-file React component for a landing page. Tailwind CSS assumed.
// Default export for easy preview in Canvas.

export default function LandingPage() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-white to-slate-50 text-slate-900">
      <header className="border-b bg-white/60 backdrop-blur sticky top-0 z-30">
        <div className="container mx-auto px-6 py-4 flex items-center justify-between">
          <div className="flex items-center gap-3">
            <div className="w-10 h-10 rounded-full bg-gradient-to-br from-rose-500 to-orange-400 flex items-center justify-center text-white font-bold">BS</div>
            <div>
              <h1 className="text-lg font-semibold">Bilingual SaaS Sales Academy</h1>
              <p className="text-xs text-slate-500">Helping Spanish-speaking & bilingual BDRs break into corporate SaaS sales</p>
            </div>
          </div>
          <nav className="flex items-center gap-3">
            <a href="#programs" className="text-sm hover:underline">Programs</a>
            <a href="#about" className="text-sm hover:underline">About</a>
            <a href="#contact" className="text-sm hover:underline">Contact</a>
            <Button className="ml-4">Join the Waitlist</Button>
          </nav>
        </div>
      </header>

      <main className="container mx-auto px-6 py-16">
        <section className="grid md:grid-cols-2 gap-10 items-center">
          <motion.div
            initial={{ opacity: 0, x: -20 }}
            animate={{ opacity: 1, x: 0 }}
            transition={{ duration: 0.6 }}
          >
            <h2 className="text-4xl md:text-5xl font-extrabold leading-tight">Turn bilingual skills into a high-paying SaaS sales career</h2>
            <p className="mt-4 text-lg text-slate-600">Real-world coaching, role-play practice, and job-ready playbooks built for Spanish-speaking and bilingual BDRs who want to break into enterprise tech sales.</p>

            <div className="mt-6 flex flex-wrap gap-3">
              <Button>Start Your Journey</Button>
              <Button variant="ghost">Book a Free Call</Button>
            </div>

            <div className="mt-8 grid grid-cols-2 gap-4">
              <Card>
                <CardContent className="flex items-start gap-3">
                  <Zap className="w-6 h-6" />
                  <div>
                    <p className="text-sm font-semibold">Fast Results</p>
                    <p className="text-xs text-slate-500">Move from first interview to offer-ready skillset.</p>
                  </div>
                </CardContent>
              </Card>
              <Card>
                <CardContent className="flex items-start gap-3">
                  <Users className="w-6 h-6" />
                  <div>
                    <p className="text-sm font-semibold">Community</p>
                    <p className="text-xs text-slate-500">Practice with peers and build a network in tech.</p>
                  </div>
                </CardContent>
              </Card>
            </div>
          </motion.div>

          <motion.div
            initial={{ opacity: 0, y: 20 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.6, delay: 0.1 }}
            className="bg-white rounded-2xl p-6 shadow-md"
          >
            <h3 className="text-xl font-semibold">What you’ll get</h3>
            <ul className="mt-4 space-y-3 text-slate-600">
              <li>• Interview & role-play coaching for enterprise sales</li>
              <li>• Bilingual outreach templates (Spanish & English)</li>
              <li>• LinkedIn profile & personal branding guidance</li>
              <li>• Tool training: Salesforce, Outreach, ZoomInfo</li>
            </ul>
            <p className="text-xs text-slate-400 mt-4">No fluff — practical, job-focused training designed by someone with enterprise sales experience.</p>
          </motion.div>
        </section>

        <section id="about" className="mt-20">
          <h3 className="text-2xl font-bold">About the Program</h3>
          <p className="mt-3 text-slate-600">This program was built to bridge the gap for Spanish-speaking talent who are excellent communicators but haven’t yet translated that skill into enterprise SaaS roles. We focus on playbooks, confidence, and real demonstrations of value that hiring managers care about.</p>

          <div className="mt-8 grid md:grid-cols-3 gap-6">
            <Card>
              <CardContent>
                <h4 className="font-semibold">1:1 Coaching</h4>
                <p className="text-sm text-slate-500 mt-2">Tailored mentorship to sharpen your pitch, role-play, and interview performance.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent>
                <h4 className="font-semibold">Group Workshops</h4>
                <p className="text-sm text-slate-500 mt-2">Live sessions, peer feedback, and mock SDR/BDR exercises in both languages.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent>
                <h4 className="font-semibold">Resources & Templates</h4>
                <p className="text-sm text-slate-500 mt-2">Script libraries, LinkedIn templates, and workbooks you can reuse every day.</p>
              </CardContent>
            </Card>
          </div>
        </section>

        <section id="programs" className="mt-16">
          <h3 className="text-2xl font-bold">Programs & Pricing</h3>
          <div className="mt-6 grid md:grid-cols-3 gap-6">
            <Card>
              <CardContent>
                <h4 className="font-semibold">Bootcamp</h4>
                <p className="text-sm text-slate-500 mt-2">4-week live cohort — outreach, role-play, and interview prep.</p>
                <div className="mt-4 flex items-center gap-3">
                  <p className="text-lg font-bold">$499</p>
                  <Button variant="ghost">Join</Button>
                </div>
              </CardContent>
            </Card>

            <Card>
              <CardContent>
                <h4 className="font-semibold">1:1 Coaching</h4>
                <p className="text-sm text-slate-500 mt-2">Personalized plan and weekly sessions.</p>
                <div className="mt-4 flex items-center gap-3">
                  <p className="text-lg font-bold">$129/month</p>
                  <Button variant="ghost">Book</Button>
                </div>
              </CardContent>
            </Card>

            <Card>
              <CardContent>
                <h4 className="font-semibold">Free Community</h4>
                <p className="text-sm text-slate-500 mt-2">Access to group practice, resources, and monthly AMA.</p>
                <div className="mt-4 flex items-center gap-3">
                  <p className="text-lg font-bold">Free</p>
                  <Button variant="ghost">Join</Button>
                </div>
              </CardContent>
            </Card>
          </div>
        </section>

        <section className="mt-16">
          <h3 className="text-2xl font-bold">Testimonials</h3>
          <div className="mt-6 grid md:grid-cols-2 gap-6">
            <Card>
              <CardContent>
                <p className="text-slate-700">"Before joining, I couldn't get past phone screens. After the bootcamp I got 3 interviews and an offer. Gracias!"</p>
                <p className="mt-3 text-xs text-slate-500">— María G., BDR</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent>
                <p className="text-slate-700">"The bilingual templates saved me hours of work and helped me close my first enterprise meeting."</p>
                <p className="mt-3 text-xs text-slate-500">— Javier R., SDR</p>
              </CardContent>
            </Card>
          </div>
        </section>

        <section id="contact" className="mt-16 mb-24">
          <h3 className="text-2xl font-bold">Contact</h3>
          <p className="mt-3 text-slate-600">Ready to get started? Join the waitlist or book a free intro call.</p>

          <div className="mt-6 grid md:grid-cols-2 gap-6">
            <form className="bg-white p-6 rounded-2xl shadow-md">
              <label className="block text-sm font-medium">Full name</label>
              <input className="mt-2 block w-full rounded-md border p-2" placeholder="Your name" />

              <label className="block text-sm font-medium mt-4">Email</label>
              <input className="mt-2 block w-full rounded-md border p-2" placeholder="you@company.com" />

              <label className="block text-sm font-medium mt-4">Message</label>
              <textarea className="mt-2 block w-full rounded-md border p-2 h-24" placeholder="How can I help?" />

              <div className="mt-4 flex items-center gap-3">
                <Button type="submit">Send</Button>
                <Button variant="ghost">Book a Call</Button>
              </div>
            </form>

            <div className="flex flex-col justify-center gap-4">
              <div className="bg-white p-6 rounded-2xl shadow-md flex items-start gap-4">
                <Mail className="w-6 h-6 text-slate-600" />
                <div>
                  <p className="font-semibold">Email</p>
                  <p className="text-xs text-slate-500">hello@bilingualsaassales.com</p>
                </div>
              </div>

              <div className="bg-white p-6 rounded-2xl shadow-md flex items-start gap-4">
                <MapPin className="w-6 h-6 text-slate-600" />
                <div>
                  <p className="font-semibold">Based in</p>
                  <p className="text-xs text-slate-500">Austin, TX</p>
                </div>
              </div>

              <div className="bg-white p-6 rounded-2xl shadow-md flex items-start gap-4">
                <Users className="w-6 h-6 text-slate-600" />
                <div>
                  <p className="font-semibold">Community</p>
                  <p className="text-xs text-slate-500">Monthly practice sessions & AMAs</p>
                </div>
              </div>
            </div>
          </div>
        </section>
      </main>

      <footer className="border-t py-6 bg-white">
        <div className="container mx-auto px-6 flex items-center justify-between">
          <p className="text-sm text-slate-500">© {new Date().getFullYear()} Bilingual SaaS Sales Academy</p>
          <div className="text-sm text-slate-500">Built with ❤️ for bilingual talent</div>
        </div>
      </footer>
    </div>
  );
}
