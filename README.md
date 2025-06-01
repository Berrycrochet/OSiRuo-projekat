# OSiRuo-projekat
Repository za OSiRuO. Studentice koje su radile na projektu: Berina Helvida, Dženana Šehić, Ajna Oparić  i Amina Kahrimanović.
# Film zona – Projekat iz OSiRuO

**Film zona** je statička web aplikacija predstavljena kao dio projekta iz predmeta *Operativni sistemi i računarstvo u oblaku*. Cilj projekta je praktično prikazati znanje iz Linux komandne linije, Docker kontejnera i cloud okruženja.

## 🎯 Cilj projekta

- Demonstracija rada sa Linux komandnom linijom
- Kreiranje i Dockerizacija statičke web aplikacije
- Deploy aplikacije na Vercel cloud platformu
- Osnovna automatizacija kroz radne skripte i build procese

## 🚀 Tehnologije

- HTML & CSS (statička web aplikacija)
- Docker
- Vercel (cloud deploy)
- GitHub

## 📂 Sadržaj aplikacije

Aplikacija se sastoji od više stranica:
- `index.html` – početna ruta `/` sa porukom dobrodošlice
- `pocetna.html`- uvod u film zonu 
- `filmovi.html` – lista filmova
- `Cjenovnik.html` – prikaz cjenovnika
- `kviz.html` – kviz o filmovima


## ⚙️ Pokretanje lokalno (Docker)

1. Build:
   ```bash
   docker build -t film-zona .
Run:
bash
docker run -d -p 8080:80 film-zona
Otvori u pregledniku: http://localhost:8080

☁️ Deploy na cloud
Deploy je urađen putem Vercel platforme.

🔗 Aplikacija dostupna na:

👉 https://o-si-ruo-projekat.vercel.app/

📁 Dockerfile (sažetak)
Dockerfile

FROM nginx:alpine
RUN rm -rf /usr/share/nginx/html/*
COPY . /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

🧠 Naučeno
Kako koristiti Docker za kreiranje i testiranje aplikacija lokalno

Razlika između lokalnog i cloud hostovanja

Osnove rada sa Vercelom i povezivanje GitHub repozitorija

Organizacija statičkih fajlova i rutiranje u web aplikaciji

📎 Linkovi
🔗 GitHub repozitorij: https://github.com/Berrycrochet/OSiRuo-projekat

🔗 Aplikacija na Vercelu: https://o-si-ruo-projekat.vercel.app/
