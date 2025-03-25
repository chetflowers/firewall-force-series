📘 **Firewall Force: The Password Heist**

### Chapter 4: Proxy Puppet

⸻

### 📍 Scene 1 – Digital Academy, Sunday Afternoon – Principal's Office

The lights buzzed faintly overhead. Principal Derwin stood behind his desk, arms crossed. Across from him sat **Beck** — a sophomore with messy hair, a cracked Chromebook, and the kind of blank expression only guilt or confusion could pull off.

> "Do you know what this is?" Derwin said, turning the screen.

The screen showed a shell command window, still faintly active:
```
sudo ./inject_null.sh -target:sysroot
```

**Beck** blinked. "That’s... not mine. I—I was doing a history report."

Nova and Jax watched silently from the hallway, tucked behind the glass door’s shadow line. Lena’s voice buzzed softly in their earpieces.

> "Zee just isolated the last command origin. It was from **Beck**’s machine. But the signature’s spoofed. This kid’s a puppet."

Zee’s voice jumped in next.  
> "And Nullroot left a backdoor open. We can get in. But we’ve got to be surgical."

> "Time to cut the strings," Nova whispered.

⸻

### 📍 Scene 2 – Rooftop HQ, 20 Minutes Later

Zee projected a network diagram across the arcade wall. Lines and nodes pulsed.

> "See this? That Chromebook is a shell host. Nullroot’s using it to bounce commands."

> "How?" Jax asked. "Remote software?"

> "Something like SSH-over-WebSocket. Except he buried it under a fake dictionary app update."

Nova winced. "That’s evil."

> "We dig in, we might expose the control IP."

Lena tapped furiously at her terminal. "We can push a false ping through the tunnel, watch for the bounce, isolate the controlling signal."

Jax grinned. "Classic echo trap."

Zee nodded. "But we only get one shot. If he sees it, he’ll shut down the node."

⸻

### 📍 Scene 3 – Covert Ops

Nova ghosted into the library. **Beck**’s Chromebook was still open on the desk.  
She plugged in a small device — Zee’s custom inline sniffer.

> "Signal injected. Tracking... tracking..."

Back at HQ, Zee and Lena watched the waveform shift. Then —

> "We’ve got him," Lena said. "Data bouncing off a proxy server in Switzerland, then tunneling through a Tor node."

> "And here’s the real signature," Zee added. "He’s using an obfuscated MAC, but we’ve got the packet delay profile. Nullroot’s not just hijacking devices — he’s mapping student accounts across the district."

> "Why?" Jax asked.

> "He’s building something," Nova said. "And we just found one of his test sites."

⸻

### 📍 Scene 4 – Payload Intercept

Firewall Force spun into action. Lena triggered a code fragment into the signal tunnel — a fake login packet with embedded trace code.

> "If he reads it, it’ll ping us back his internal IP."

Zee counted the beats. "1... 2... 3... Got it."

On-screen: `192.168.45.109`

> "Local device. Nullroot’s not remote today. He’s on-site."

Nova’s jaw clenched. "Then we smoke him out."

They all looked at the screen.  
A new message blinked into view:
```
Not bad, Firewall Force.
You pull one string, but I’ve got dozens more.
– N
```

> "Let’s cut them all," Jax said.

⸻

**End of Chapter 4**
