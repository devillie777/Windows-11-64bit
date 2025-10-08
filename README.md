Current runner version: '2.328.0'

Runner Image Provisioner

Operating System

Runner Image

GITHUB_TOKEN Permissions

Secret source: Actions

Prepare workflow directory

Prepare all required actions

Complete job name: secure-rdp

Run # Enable Remote Desktop and disable Network Level Authentication (if needed)

No rules match the specified criteria.

Ok.

Run Add-Type -AssemblyName System.Security

Name Enabled Description
---- ------- -----------
RDP  True    

Run $tsUrl = "https://pkgs.tailscale.com/stable/tailscale-setup-1.82.0-amd64.msi"

Run # Bring up Tailscale with the provided auth key and set a unique hostname
To authenticate, visit:
	https://login.tailscale.com/a/e518b4f01e10c
Success.

Run Write-Host Application "Windows 11 64bit IP: $env:Windows 11 64bit"
  
Tailscale IP: 100.103.8.7

TCP connectivity successful!

Run Write-Host "`n=== RDP ACCESS ==="
  
=== RDP ACCESS ===
Address: 100.103.8.7
Username: RDP
Password: User: RDP | Password: 8in032;P=+SgLI\z
==================
[10/08/2025 07:41:29] RDP Active - Use Ctrl+C in workflow to terminate

Windows 11 64-bit RDP Game Streaming Setup
Ito ay isang Windows 11 64-bit operating system na naka-configure para sa Remote Desktop Protocol (RDP), na nagbibigay-daan sa mga user na maglaro ng PC games nang remote gamit lamang ang internet connection. Sa pamamagitan ng RDP, maaaring kumonekta mula sa ibang device (hal. laptop, tablet, o low-end PC) at gamitin ang kapangyarihan ng host PC para magpatakbo ng mga laro. Sinusuportahan nito ang high-speed na koneksyon para sa mas mabilis na input response at mas malinaw na video output, depende sa bandwidth. Mainam ito para sa mga user na gustong maglaro kahit malayo sa kanilang gaming PC.

Key Features:

Windows 11 64-bit compatibility

Fully functional RDP access

Supports game streaming via RDP (with optimization)

Allows remote gameplay from anywhere with internet

Ideal for high-spec PC gaming via low-end client devices

Note: Ang RDP ay hindi kasing-optimal ng mga dedicated game streaming services tulad ng Steam Remote Play, NVIDIA GeForce NOW, o Parsec, pero maaari pa rin itong gamitin kung tama ang configuration (tulad ng pag-enable ng GPU acceleration at tamang network setup).
