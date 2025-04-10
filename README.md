# Good-Nurseimport React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

export default function Home() {
  return (
    <main className="min-h-screen bg-white text-gray-800">
      <header className="bg-blue-600 text-white py-6 shadow-md">
        <div className="container mx-auto px-4 flex justify-between items-center">
          <h1 className="text-2xl font-bold"> GOOD NURSE</h1>
          <nav className="space-x-4">
            <a href="#about" className="hover:underline">About</a>
            <a href="#resources" className="hover:underline">Resources</a>
            <a href="#join" className="hover:underline">Join</a>
            <a href="#contact" className="hover:underline">Contact</a>
          </nav>
        </div>
      </header>

      <section className="text-center py-20 bg-gray-100">
        <h2 className="text-4xl font-bold mb-4">Welcome to  GOOD NURSE</h2>
        <p className="text-lg mb-6">Empowering nurses around the world with knowledge and community.</p>
        <Button className="bg-blue-600 text-white px-6 py-2 rounded-full">Join Us Now</Button>
      </section>

      <section id="about" className="py-16 px-4 container mx-auto">
        <h3 className="text-2xl font-bold mb-4">About Us</h3>
        <p>
           GOOD NURSE is a global platform created by nurses for nurses. We aim to support,
          educate, and connect nurses across all backgrounds through free knowledge-sharing.
        </p>
      </section>

      <section id="resources" className="py-16 px-4 bg-gray-100 container mx-auto">
        <h3 className="text-2xl font-bold mb-4">Resources</h3>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          <Card>
            <CardContent className="p-4">
              <h4 className="text-lg font-semibold">Nursing Handouts</h4>
              <p>Downloadable and printable PDF guides for daily nursing tasks.</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-4">
              <h4 className="text-lg font-semibold">Articles & Tips</h4>
              <p>Helpful nursing knowledge, updated weekly.</p>
            </CardContent>
          </Card>
        </div>
      </section>

      <section id="join" className="py-16 px-4 container mx-auto">
        <h3 className="text-2xl font-bold mb-4">Join Our Community</h3>
        <form className="max-w-lg mx-auto space-y-4">
          <input type="text" placeholder="Full Name" className="w-full p-2 border rounded" />
          <input type="email" placeholder="Email Address" className="w-full p-2 border rounded" />
          <Button className="bg-blue-600 text-white w-full">Register</Button>
        </form>
      </section>

      <section id="contact" className="py-16 px-4 bg-gray-100 container mx-auto">
        <h3 className="text-2xl font-bold mb-4">Contact Us</h3>
        <p>Email: support@goodnurse.com</p>
      </section>

      <footer className="bg-blue-600 text-white py-4 text-center">
        &copy; 2025  GOOD NURSE. All rights reserved.
      </footer>
    </main>
  );
}
