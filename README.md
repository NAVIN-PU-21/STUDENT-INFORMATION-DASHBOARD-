# STUDENT-INFORMATION-DASHBOARD-
Creating a 2nd year mini project for my college about student information database , designed to efficiently manage and display student data. It integrates a user-friendly interface with a robust database system to store, retrieve, and update student information in real-time.
   student login #student login interface
   import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Input } from "@/components/ui/input";
import { Button } from "@/components/ui/button";
import { Lock, User } from "lucide-react";
import Image from "next/image";

export default function LoginPage() {
  return (
    <div className="relative h-screen w-screen flex items-center justify-center bg-gray-100">
      {/* Background Image */}
      <Image
        src="/background.jpg" // updated background image path
        alt="Background"
        layout="fill"
        objectFit="cover"
        className="z-0"
      />

      {/* Overlay */}
      <div className="absolute inset-0 bg-black/30 z-10" />

      {/* Login Card */}
      <Card className="relative z-20 flex w-[400px] shadow-2xl rounded-2xl overflow-hidden">
        <div className="w-1/3 flex flex-col items-center justify-center bg-gradient-to-b from-blue-500 to-purple-500 text-white p-4">
          <Image
            src="/veltech-logo.png" // replace with actual logo path
            alt="Vel Tech Logo"
            width={80}
            height={80}
            className="mb-4"
          />
          <h2 className="text-sm font-semibold text-center">Vel Tech High Tech</h2>
        </div>
        <CardContent className="w-2/3 p-6 flex flex-col justify-center">
          <h1 className="text-xl font-bold mb-6 text-center">WELCOME BACK</h1>
          <div className="space-y-4">
            <div className="relative">
              <Input placeholder="VH.no" className="pl-10" />
              <User className="absolute left-2 top-2.5 h-5 w-5 text-gray-400" />
            </div>
            <div className="relative">
              <Input type="password" placeholder="Password" className="pl-10" />
              <Lock className="absolute left-2 top-2.5 h-5 w-5 text-gray-400" />
            </div>
            <Button className="w-full bg-gradient-to-r from-blue-500 to-purple-500 text-white font-semibold">
              LOGIN
            </Button>
          </div>
        </CardContent>
      </Card>
    </div>
  );
}
