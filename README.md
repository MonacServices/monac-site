import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mail, Linkedin } from "lucide-react";

export default function HomePage() {
  return (
    <main className="min-h-screen bg-gray-50 text-gray-800 p-6">
      <section className="max-w-5xl mx-auto grid gap-6">
        {/* Hero Section */}
        <div className="text-center py-16">
          <h1 className="text-4xl font-bold mb-4 text-blue-900">
            Monac IT Audit, Compliance and Risk Advisory
          </h1>
          <p className="text-lg text-gray-700 max-w-2xl mx-auto">
            Helping organizations manage IT risk, meet compliance requirements,
            and strengthen internal controls with expert, independent advice.
          </p>
          <div className="mt-6 flex justify-center gap-4">
            <Button>
              <Mail className="mr-2 h-4 w-4" /> Contact
            </Button>
            <Button variant="outline">
              <Linkedin className="mr-2 h-4 w-4" /> LinkedIn
            </Button>
          </div>
        </div>

        {/* About Section */}
        <Card className="bg-white shadow-xl rounded-2xl">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold text-blue-800 mb-2">About</h2>
            <p>
              Monac is a one-man consultancy founded by an experienced IT auditor
              and compliance advisor. I work closely with clients to understand
              their specific challenges and deliver tailored, pragmatic
              solutions that meet regulatory and operational needs.
            </p>
          </CardContent>
        </Card>

        {/* Services Section */}
        <Card className="bg-white shadow-xl rounded-2xl">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold text-blue-800 mb-4">Services</h2>
            <ul className="list-disc list-inside space-y-2">
              <li>
                <strong>IT Audit</strong> – IT General Controls, application audits,
                ISO 27001 readiness assessments
              </li>
              <li>
                <strong>Compliance</strong> – GDPR, NIS2, DNB/AFM frameworks,
                regulatory gap analysis
              </li>
              <li>
                <strong>Risk Advisory</strong> – Information risk assessments,
                policy development, internal controls strengthening
              </li>
            </ul>
          </CardContent>
        </Card>

        {/* Contact Section */}
        <Card className="bg-white shadow-xl rounded-2xl">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold text-blue-800 mb-2">Contact</h2>
            <p>
              Get in touch for a free consultation or to learn more about how
              Monac can support your organization.
            </p>
            <p className="mt-2">
              📧 <a className="text-blue-600 underline" href="mailto:info@monacadvisory.com">info@monacadvisory.com</a>
            </p>
            <p>
              🔗 <a className="text-blue-600 underline" href="https://www.linkedin.com/in/your-profile">LinkedIn</a>
            </p>
          </CardContent>
        </Card>
      </section>
    </main>
  );
}
