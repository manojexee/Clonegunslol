# Clonegunslol
import React from "react";
import { motion } from "framer-motion";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Input } from "@/components/ui/input";

const GunsLolClone = () => {
  return (
    <div className="bg-gray-900 text-white min-h-screen flex flex-col items-center">
      {/* Header Section */}
      <header className="w-full p-4 bg-gray-800 shadow-lg flex justify-between items-center">
        <h1 className="text-2xl font-bold">Guns.LOL Clone</h1>
        <nav>
          <ul className="flex space-x-4">
            <li>
              <a href="#play" className="hover:underline">Play</a>
            </li>
            <li>
              <a href="#leaderboard" className="hover:underline">Leaderboard</a>
            </li>
            <li>
              <a href="#about" className="hover:underline">About</a>
            </li>
          </ul>
        </nav>
      </header>

      {/* Hero Section */}
      <section className="mt-10 text-center">
        <motion.h2
          initial={{ opacity: 0, y: -50 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.8 }}
          className="text-4xl font-extrabold"
        >
          Welcome to the Ultimate Shooting Game
        </motion.h2>
        <p className="text-lg mt-4">
          Quick matches. Exciting gameplay. Compete globally!
        </p>
        <Button className="mt-6 bg-green-500 hover:bg-green-600">
          Start Playing
        </Button>
      </section>

      {/* Game Embed Section */}
      <section id="play" className="mt-12 w-full flex justify-center">
        <iframe
          title="Guns Game"
          src="https://example-game-url.com"
          className="w-3/4 h-[500px] border-2 border-gray-700 rounded-lg"
        ></iframe>
      </section>

      {/* Leaderboard Section */}
      <section id="leaderboard" className="mt-12 w-3/4">
        <h3 className="text-2xl font-bold mb-4">Leaderboard</h3>
        <Card className="mb-4">
          <CardContent>
            <div className="flex justify-between">
              <span>Player1</span>
              <span>1200 points</span>
            </div>
          </CardContent>
        </Card>
        <Card className="mb-4">
          <CardContent>
            <div className="flex justify-between">
              <span>Player2</span>
              <span>1100 points</span>
            </div>
          </CardContent>
        </Card>
      </section>

      {/* Footer Section */}
      <footer id="about" className="mt-12 p-6 bg-gray-800 w-full text-center">
        <p>
          Guns.LOL Clone created for fun and learning. Inspired by <strong>guns.lol</strong>.
        </p>
      </footer>
    </div>
  );
};

export default GunsLolClone;
 
