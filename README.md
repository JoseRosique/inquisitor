<!DOCTYPE html>
<html>
<body>
  <h1>Inquisitor Project</h1>

  <h2>Mandatory Part</h2>
  <h3>Environment Setup</h3>
  <ul>
    <li>If you choose to work with a virtual machine, include a file called <code>signature.txt</code> in the delivery repository. This file should contain the checksum of your machine's <code>.vdi</code> file. During evaluation, the repository's signature will be compared with the real signature of your machine. If they do not match, your score will be marked as 0.</li>
    <li>If you opt to work with containers, include the code of your program, along with a Dockerfile or docker-compose.yaml file. Additionally, provide a Bash script named <code>start.sh</code> that starts the entire environment without user intervention.</li>
  </ul>

  <h3>Program Description</h3>
  <p>The program, "inquisitor," has the following characteristics:</p>
  <ul>
    <li>It receives four parameters: <code>&lt;IP-src&gt; &lt;MAC-src&gt; &lt;IP-target&gt; &lt;MAC-target&gt;</code>.</li>
    <li>The program is capable of performing ARP poisoning in both directions (full duplex).</li>
    <li>When the attack is stopped (CTRL+C), the program restores the ARP tables.</li>
    <li>It only works with IPv4 addresses.</li>
    <li>The program can intercept the traffic resulting from the login to an FTP server.</li>
    <li>Real-time display of the names of the files exchanged between the client and the FTP server.</li>
    <li>The program handles all input errors and never stops unexpectedly.</li>
    <li>The libpcap library is used to sniff packets, allowing the use of any programming language that implements it (e.g., C, C++, Python, etc.).</li>
  </ul>

  <h2>Bonus Part</h2>
  <p>The evaluation of the bonuses will be done only if the mandatory part is perfect. Otherwise, the bonuses will be ignored.</p>
  <ul>
    <li>"Verbose" (-v) mode: In this mode, the program shows all FTP traffic, not just filenames.</li>
  </ul>

  <p>Good luck with your project!</p>
</body>
</html>
