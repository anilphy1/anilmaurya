# ====== STEP 1: Configure Git ======
git config --global user.name "Anil Maurya"
git config --global user.email "your.email@example.com"

# ====== STEP 2: Create folder and files ======
mkdir my-website
cd my-website

# Create a simple homepage
cat > index.html <<'EOF'
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Anil Maurya | Physics Portfolio</title>
</head>
<body style="font-family:sans-serif; text-align:center; margin-top:100px;">
  <h1>Hello, I'm Anil Maurya 👋</h1>
  <p>Master’s Student in Physics at the University of Camerino, Italy</p>
  <p>Passionate about Quantum Physics, Particle Physics, and Astrophysics</p>
  <p><a href="https://www.linkedin.com/in/anil-maurya-2860b2206">LinkedIn</a></p>
</body>
</html>
EOF

# ====== STEP 3: Initialize Git ======
git init
git add .
git commit -m "Initial commit"

# ====== STEP 4: Connect to GitHub ======
git branch -M main
git remote add origin https://github.com/your-username/your-username.github.io.git
git push -u origin main

# ====== STEP 5: Done! ======
echo "✅ Site uploaded! Enable GitHub Pages in Settings → Pages → Source → main / root."
echo "Then visit 👉 https://your-username.github.io"
