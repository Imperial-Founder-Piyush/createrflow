"use client";
import React, { useState } from 'react';

export default function Home() {
  const [username, setUsername] = useState('');

  return (
    <div style={{ backgroundColor: '#050505', color: '#fff', height: '100vh', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', fontFamily: 'sans-serif', textAlign: 'center', padding: '20px' }}>
      <h1 style={{ fontSize: '3rem', fontWeight: '800', marginBottom: '10px' }}>
        Creater<span style={{ color: '#3b82f6' }}>Flow</span>
      </h1>
      <p style={{ fontSize: '1.1rem', color: '#a1a1aa', marginBottom: '30px' }}>
        अपना हैंडल डालें और 2 मिनट में अपनी दुकान लाइव करें।
      </p>
      
      <div style={{ display: 'flex', gap: '10px', flexWrap: 'wrap', justifyContent: 'center' }}>
        <input 
          type="text" 
          placeholder="Instagram handle" 
          value={username}
          onChange={(e) => setUsername(e.target.value)}
          style={{ padding: '15px', borderRadius: '10px', border: '1px solid #333', backgroundColor: '#111', color: '#fff', width: '250px' }}
        />
        <button 
          style={{ padding: '15px 30px', backgroundColor: '#3b82f6', color: '#fff', border: 'none', borderRadius: '10px', cursor: 'pointer', fontWeight: '600' }}>
          Store बनायें
        </button>
      </div>
    </div>
  );
}
# createrflow
