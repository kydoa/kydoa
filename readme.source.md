```aura width=860 height=200
<div style={{
 width: '100%', height: '100%', background: '#08080c',
 display: 'flex', alignItems: 'center', fontFamily: 'Inter',
 position: 'relative', overflow: 'hidden', borderRadius: 16,
 border: '1px solid rgba(255,255,255,0.14)'
}}>

 <style>
   {`
     @keyframes float-slow {
       0%, 100% { transform: translateX(0px); opacity: 0.8; }
       50% { transform: translateX(350px); opacity: 1.2; }
     }
     @keyframes float-medium {
       0%, 100% { transform: translateX(0px); opacity: 0.7; }
       50% { transform: translateX(-250px); opacity: 1.1; }
     }
     @keyframes float-fast {
       0%, 100% { transform: translateX(0px); opacity: 0.9; }
       50% { transform: translateX(200px); opacity: 0.6; }
     }
     @keyframes float-diagonal {
       0%, 100% { transform: translateX(0px); opacity: 0.75; }
       50% { transform: translateX(300px); opacity: 1.0; }
     }
     @keyframes float-wave {
       0%, 100% { transform: translateX(0px); opacity: 0.65; }
       33% { transform: translateX(-160px); opacity: 0.9; }
       66% { transform: translateX(80px); opacity: 1.0; }
     }
     @keyframes float-pulse {
       0%, 100% { transform: scale(1); opacity: 0.8; }
       50% { transform: scale(1.3); opacity: 0.4; }
     }
     #glow-1 { animation: float-slow 8s ease-in-out infinite; }
     #glow-2 { animation: float-medium 12s ease-in-out infinite; }
     #glow-3 { animation: float-fast 9s ease-in-out infinite; }
     #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
     #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }
     #glow-6 { animation: float-diagonal 10s ease-in-out infinite; }
     #glow-7 { animation: float-wave 13s ease-in-out infinite; }
     #glow-8 { animation: float-pulse 7s ease-in-out infinite; }
   `}
 </style>

 <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
   <defs>
     <radialGradient id="g1" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stopColor="rgba(255,255,255,0.30)" />
      <stop offset="40%" stopColor="rgba(190,190,190,0.16)" />
      <stop offset="70%" stopColor="rgba(190,190,190,0)" />
     </radialGradient>
     <radialGradient id="g2" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stopColor="rgba(225,225,225,0.22)" />
      <stop offset="45%" stopColor="rgba(160,160,160,0.12)" />
      <stop offset="70%" stopColor="rgba(160,160,160,0)" />
     </radialGradient>
     <radialGradient id="g3" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stopColor="rgba(235,235,235,0.18)" />
      <stop offset="50%" stopColor="rgba(175,175,175,0.08)" />
      <stop offset="70%" stopColor="rgba(175,175,175,0)" />
     </radialGradient>
     <radialGradient id="g4" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stopColor="rgba(210,210,210,0.14)" />
      <stop offset="70%" stopColor="rgba(210,210,210,0)" />
     </radialGradient>
     <radialGradient id="g5" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stopColor="rgba(170,170,170,0.16)" />
      <stop offset="70%" stopColor="rgba(170,170,170,0)" />
     </radialGradient>
     <radialGradient id="g6" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stopColor="rgba(255,255,255,0.22)" />
      <stop offset="45%" stopColor="rgba(190,190,190,0.10)" />
      <stop offset="70%" stopColor="rgba(190,190,190,0)" />
     </radialGradient>
     <radialGradient id="g7" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stopColor="rgba(225,225,225,0.16)" />
      <stop offset="50%" stopColor="rgba(155,155,155,0.08)" />
      <stop offset="70%" stopColor="rgba(155,155,155,0)" />
     </radialGradient>
     <radialGradient id="g8" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stopColor="rgba(215,215,215,0.14)" />
      <stop offset="50%" stopColor="rgba(145,145,145,0.06)" />
      <stop offset="70%" stopColor="rgba(145,145,145,0)" />
     </radialGradient>
   </defs>

   <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />
   <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />
   <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />
   <ellipse id="glow-4" cx="550" cy="250" rx="150" ry="120" fill="url(#g4)" />
   <ellipse id="glow-5" cx="750" cy="250" rx="130" ry="110" fill="url(#g5)" />
   <ellipse id="glow-6" cx="300" cy="240" rx="180" ry="140" fill="url(#g6)" />
   <ellipse id="glow-7" cx="490" cy="230" rx="220" ry="170" fill="url(#g7)" />
   <ellipse id="glow-8" cx="590" cy="250" rx="150" ry="130" fill="url(#g8)" />
 </svg>

 <div style={{
   position: 'absolute', left: 48, top: 52, width: 96, height: 96,
  borderRadius: 48, background: 'linear-gradient(135deg, #444444, #111111)',
   display: 'flex', alignItems: 'center', justifyContent: 'center',
 }}>
   <img src={(github && github.user && github.user.avatarUrl) || 'https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png'} width={88} height={88} style={{ borderRadius: 44 }} />
 </div>

 <div style={{ display:'flex', flexDirection:'column', marginLeft:168, gap:8, zIndex: 10 }}>
   <div style={{ display:'flex', fontSize:38, fontWeight:800, color:'#ffffff', letterSpacing:'-1px', lineHeight:1 }}>
     {'Daniel Scheuermann · KYDOA'}
   </div>
  <div style={{ display:'flex', fontSize:15, color:'rgba(220,220,220,0.72)', fontWeight:400, letterSpacing:'0.3px' }}>
     {'Software Engineer & DevOps · Technology Enthusiast · Multilingual'}
      </div>
    <div style={{ display:'flex', gap:20, marginTop:4 }}>
      <div style={{ display:'flex', alignItems:'center', gap:5 }}>
        <div style={{ width:8, height:8, borderRadius:4, background:'#ffffff' }} />
        <span style={{ fontSize:12, color:'rgba(220,220,220,0.72)', fontWeight:600 }}>
          {github?.stats?.totalRepos ?? '0'} Repositories
        </span>
      </div>
      <div style={{ display:'flex', alignItems:'center', gap:5 }}>
        <div style={{ width:8, height:8, borderRadius:4, background:'#ffffff' }} />
        <span style={{ fontSize:12, color:'rgba(220,220,220,0.72)', fontWeight:600 }}>
          {github?.user?.followers ?? '0'} Followers
        </span>
      </div>
      <div style={{ display:'flex', alignItems:'center', gap:5 }}>
        <div style={{ width:8, height:8, borderRadius:4, background:'#ffffff' }} />
        <span style={{ fontSize:12, color:'rgba(220,220,220,0.72)', fontWeight:600 }}>
          {github?.stats?.totalStars ?? '0'} Stars
        </span>
      </div>
      <div style={{ display:'flex', alignItems:'center', gap:5 }}>
        <div style={{ width:8, height:8, borderRadius:4, background:'#ffffff' }} />
        <span style={{ fontSize:12, color:'rgba(220,220,220,0.72)', fontWeight:600 }}>
          {github?.stats?.totalCommits ?? '0'} Commits
        </span>
      </div>
    </div>
   <div style={{ display:'flex', gap:8, marginTop:6 }}>
     {['Java', 'C', 'SQL', 'C++', 'Python'].map(function(tag) {
       return (
         <div key={tag} style={{
           display:'flex', padding:'4px 12px', borderRadius:20,
           background:'rgba(255,255,255,0.05)', border:'1px solid rgba(255,255,255,0.14)',
           color:'rgba(235,235,235,0.82)', fontSize:12, fontWeight:600,
         }}>{tag}</div>
       );
     })}
   </div>
 </div>
</div>
```

```aura width=860 height=110
<div style={{
  width: '100%', height: '100%', background: '#08080c',
  display: 'flex', alignItems: 'center', justifyContent: 'space-around',
  fontFamily: 'Inter', borderRadius: 16,
  border: '1px solid rgba(255,255,255,0.05)', padding: '0 40px', boxSizing: 'border-box',
}}>
  {[
    { color: '#ffffff', label: 'Open Source', sub: 'All Major Projects Public' },
    { color: '#ffffff', label: 'Resource Efficient', sub: 'Built for Constrained Hardware' },
    { color: '#ffffff', label: 'Privacy-First', sub: 'Local AI — No Cloud Dependency' },
    { color: '#ffffff', label: 'Self-Hosted Culture', sub: 'Local Network & Infrastructure' },
  ].map(function(item) {
    return (
      <div key={item.label} style={{ display: 'flex', flexDirection: 'column', alignItems: 'center', gap: 6, maxWidth: 185 }}>
        <div style={{ width: 10, height: 10, borderRadius: 5, background: item.color }} />
        <span style={{ fontSize: 13, fontWeight: 700, color: '#ffffff', textAlign: 'center' }}>{item.label}</span>
        <span style={{ fontSize: 11, color: 'rgba(235,235,235,0.82)', textAlign: 'center', lineHeight: 1.4 }}>{item.sub}</span>
      </div>
    );
  })}
</div>
```

```aura width=860 height=138
(function() {
 var categories = [
  { title: 'Languages', color: '#f5f5f5', items: ['Java', 'C', 'SQL', 'Assembly', 'Prolog', 'SystemVerilog', 'C++', 'Python', 'Jupyter'] },
  { title: 'Tools', color: '#b8b8b8', items: ['Docker', 'ProxmoxVE', 'Prometheus', 'Wordpress', 'Grafana', 'Nginx', 'Forgejo', 'DNS', 'VPN'] },
 ];

 return (
   <div style={{
     width: '100%', height: '100%',
     background: '#08080c',
     display: 'flex', flexDirection: 'column',
     fontFamily: 'Inter', padding: '18px 32px', gap: 14,
    borderRadius: 16, border: '1px solid rgba(255,255,255,0.14)',
     position: 'relative', overflow: 'hidden',
   }}>

     <style>
       {`
         @keyframes float-slow {
           0%, 100% { transform: translateX(0px); opacity: 0.8; }
           50% { transform: translateX(350px); opacity: 1.2; }
         }
         @keyframes float-medium {
           0%, 100% { transform: translateX(0px); opacity: 0.7; }
           50% { transform: translateX(-250px); opacity: 1.1; }
         }
         @keyframes float-fast {
           0%, 100% { transform: translateX(0px); opacity: 0.9; }
           50% { transform: translateX(200px); opacity: 0.6; }
         }
         @keyframes float-diagonal {
           0%, 100% { transform: translateX(0px); opacity: 0.75; }
           50% { transform: translateX(300px); opacity: 1.0; }
         }
         @keyframes float-wave {
           0%, 100% { transform: translateX(0px); opacity: 0.65; }
           33% { transform: translateX(-160px); opacity: 0.9; }
           66% { transform: translateX(80px); opacity: 1.0; }
         }
         @keyframes float-pulse {
           0%, 100% { transform: scale(1); opacity: 0.8; }
           50% { transform: scale(1.3); opacity: 0.4; }
         }
         #glow-1 { animation: float-slow 9s ease-in-out infinite; }
         #glow-2 { animation: float-medium 12s ease-in-out infinite; }
         #glow-3 { animation: float-fast 8s ease-in-out infinite; }
         #glow-4 { animation: float-diagonal 11s ease-in-out infinite reverse; }
         #glow-5 { animation: float-wave 14s ease-in-out infinite reverse; }
         #glow-6 { animation: float-pulse 6s ease-in-out infinite; }
       `}
     </style>

     <svg width="860" height="138" style={{ position: 'absolute', top: 0, left: 0 }}>
       <defs>
         <radialGradient id="g1" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(255,255,255,0.22)" />
           <stop offset="42%" stopColor="rgba(180,180,180,0.10)" />
           <stop offset="70%" stopColor="rgba(180,180,180,0)" />
         </radialGradient>
         <radialGradient id="g2" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(220,220,220,0.18)" />
           <stop offset="45%" stopColor="rgba(160,160,160,0.08)" />
           <stop offset="70%" stopColor="rgba(160,160,160,0)" />
         </radialGradient>
         <radialGradient id="g3" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(230,230,230,0.14)" />
           <stop offset="50%" stopColor="rgba(170,170,170,0.06)" />
           <stop offset="70%" stopColor="rgba(170,170,170,0)" />
         </radialGradient>
         <radialGradient id="g4" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(200,200,200,0.10)" />
           <stop offset="70%" stopColor="rgba(200,200,200,0)" />
         </radialGradient>
         <radialGradient id="g5" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(160,160,160,0.12)" />
           <stop offset="70%" stopColor="rgba(160,160,160,0)" />
         </radialGradient>
         <radialGradient id="g6" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(190,190,190,0.10)" />
           <stop offset="70%" stopColor="rgba(190,190,190,0)" />
         </radialGradient>
       </defs>
       <ellipse id="glow-1" cx="170" cy="168" rx="260" ry="170" fill="url(#g1)" />
       <ellipse id="glow-2" cx="320" cy="178" rx="220" ry="140" fill="url(#g2)" />
       <ellipse id="glow-3" cx="460" cy="178" rx="190" ry="130" fill="url(#g3)" />
       <ellipse id="glow-4" cx="590" cy="188" rx="160" ry="110" fill="url(#g4)" />
       <ellipse id="glow-5" cx="750" cy="188" rx="140" ry="100" fill="url(#g5)" />
       <ellipse id="glow-6" cx="420" cy="138" rx="100" ry="80" fill="url(#g6)" />
     </svg>

    <div style={{ display:'flex', fontSize:10, fontWeight:700, color:'rgba(210,210,210,0.5)', letterSpacing:'3px' }}>
       TECH STACK
     </div>
     <div style={{ display:'flex', flexDirection:'column', gap:14 }}>
       {categories.map(function(cat) {
         return (
           <div key={cat.title} style={{ display:'flex', alignItems:'center', gap:16 }}>
             <div style={{ display:'flex', fontSize:10, fontWeight:700, color:cat.color, letterSpacing:'1px', width:80 }}>
               {cat.title.toUpperCase()}
             </div>
             <div style={{ display:'flex', flexWrap:'wrap', gap:7 }}>
               {cat.items.map(function(item) {
                 return (
                   <div key={item} style={{
                     display:'flex', padding:'4px 13px', borderRadius:6,
                     background:'rgba(255,255,255,0.05)', border:'1px solid rgba(255,255,255,0.12)',
                     color:'rgba(235,235,235,0.82)', fontSize:12, fontWeight:600,
                   }}>{item}</div>
                 );
               })}
             </div>
           </div>
         );
       })}
     </div>
   </div>
 );
})()
```

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=kydoa&theme=dark" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=kydoa&theme=dark&utcOffset=8" />
</p>

```aura width=120 height=44 link="https://www.linkedin.com/in/kydoa/" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/d-scheuermann/d-scheuermann/refs/heads/main/icons/linkedin.svg"
  text="Linkedin"
  backgroundColor="#111111"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#cccccc' },
    { offset: '60%', color: '#ffffff' },
    { offset: '80%', color: '#000000' },
    { offset: '100%', color: '#666666' },
  ]}
/>
```

```aura width=120 height=44 link="https://chat.kydoa.com/" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/d-scheuermann/d-scheuermann/refs/heads/main/icons/whatsapp.svg"
  text="WhatsApp"
  backgroundColor="#111111"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#cccccc' },
    { offset: '60%', color: '#ffffff' },
    { offset: '80%', color: '#000000' },
    { offset: '100%', color: '#666666' },
  ]}
/>
```

```aura width=120 height=44 link="https://kydoa.com/" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/d-scheuermann/d-scheuermann/refs/heads/main/icons/globe.svg"
  text="Kydoa"
  backgroundColor="#111111"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#cccccc' },
    { offset: '60%', color: '#ffffff' },
    { offset: '80%', color: '#000000' },
    { offset: '100%', color: '#666666' },
  ]}
/>
```

```aura width=120 height=44 link="https://github.com/kydoa" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/d-scheuermann/d-scheuermann/refs/heads/main/icons/github.svg"
  text="GitHub"
  backgroundColor="#111111"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#cccccc' },
    { offset: '60%', color: '#ffffff' },
    { offset: '80%', color: '#000000' },
    { offset: '100%', color: '#666666' },
  ]}
/>
```

```aura width=120 height=44 link="mailto:daniel@kydoa.com" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/d-scheuermann/d-scheuermann/refs/heads/main/icons/mail.svg"
  text="Email"
  backgroundColor="#111111"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#cccccc' },
    { offset: '60%', color: '#ffffff' },
    { offset: '80%', color: '#000000' },
    { offset: '100%', color: '#666666' },
  ]}
/>
```
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:ffffff,100:ffffff&height=135&section=footer&animation=fadeIn" />