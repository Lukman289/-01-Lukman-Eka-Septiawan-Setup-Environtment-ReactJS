This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Laporan Praktikum
|    |  Pemrograman Berbasis Framework 2024  |
| ------------- | ------------- |
| NIM | 2241720049 |
| Nama | Lukman Eka Septiawan |
| Kelas | TI-3A |

### Jawaban Soal Praktikum 1
1. Jelaskan kegunaan masing-masing dari Git, VS Code, dan NodeJS yang telah Anda install 
pada sesi praktikum ini! 

#### GIT
GIT adalah Version Control System yang dapat membantu developer dalam mengelola suatu project seperti melihat perubahan kode yang sudah dibuat.

#### VS Code
VS Code merupakan code editor yang digunakan untuk mengembangkan sebuah aplikasi.

#### NodeJS
NodeJS merupakan sebuah runtime environment yang dapat menjalankan program secara bersamaan tanpa menunggu satu proses selesai. 

2. Buktikan dengan screenshoot yang menunjukkan bahwa masing-masing tools tersebut telah berhasil terinstall di perangkat Anda!

#### GIT
![GIT Installed](public\img\p1-2_git.png)

#### VS Code
![VS Code Installed](public\img\p1-2_vsc.png)

#### NodeJS
![NodeJS Installed](public\img\p1-2_node.png)

### Jawaban Soal Praktikum 2
1. Pada Langkah ke-2, setelah membuat proyek baru menggunakan Next.js, terdapat beberapa istilah yang muncul. Jelaskan istilah tersebut, TypeScript, ESLint, Tailwind CSS, App Router, Import alias, App router, dan Turbopack! 

- TypeScript adalah superset dari JavaScript yang menambahkan static typing pada JavaScript untuk meningkatkan skalabilitas kode.
- ESLint adalah linter untuk membantu memastikan konsistensi kode dan mencegah bug.
- Tailwind CSS merupakan framework CSS yang memungkinkan styling langsung pada HTML tanpa membuat banyak file CSS.
- App Router adalah fitur routing yang ada di NextJS.
- Import alias merupakan sebuah fitur untuk menghindari penamaan import yang panjang dalam proyek JavaScript.
- Turbopack merupakan bundler yang ditujukan untuk meningkatkan kevepatan dan efisiensi dalam membangun aplikasi web.

2. Apa saja kegunaan folder dan file yang ada pada struktur proyek React yang tampil pada gambar pada tahap percobaan ke-3! 

- public adalah folder yang dapat diakses oleh pengguna seperti file gambar.
- src adalah folder yang digunakan untuk menyimpan file yang digunakan untuk menangani server seperti route, controller, model, dan view.
- .gitignore merupakan file yang berisi berkas dan folder yang tidak boleh diupload ke server (git).
- package.json adalah file yang berisi data dan detail semua dependensi yang terinstall pada proyek/aplikasi.
- eslint.config.mjs adalah file konfigurasi dari ESLint yang digunkan untuk mengatur aturan pada proyek.
- readme.md merupakan file berisi tentang informasi proyek yang dikembangkan.
- next-env.d.ts adalah file yang digunakan untuk memastikan bahwa typescript dapat mengenali fitur-fitur spesifik dari Next.js.
- next.config.ts merupakan file konfigurasi pada proyek Next.js.
- package-lock.json merupakan file yang digunakan untuk mengamankan depedensi agar tetap konsiste.
- postcss.config.mjs adalah file yang digunakan untuk mengolah file CSS dan memproses utility classess untuk proyek yang menggunakan TailwindCSS.
- tailwind.config.ts adalah file konfigurasi untuk TailwindCSS.
- tsconfig.json adalah file konfigurasi untuk TypeScript.


3. Buktikan dengan screenshoot yang menunjukkan bahwa tahapan percobaan di atas telah berhasil Anda lakukan!

#### Install NPM
![NPM Installed](public\img\p2-3_npm.png)

#### Struktur NPM
![NPM Structure](public\img\p2-3_struktur.png)

#### Running NPM
![NPM Run Dev](public\img\p2-3_npm-run.png)

### Jawaban Soal Praktikum 3
1. Buktikan dengan screenshoot yang menunjukkan bahwa tahapan percobaan di atas telah berhasil Anda lakukan!

Perubahan page.txt
~~~typescript
import Image from "next/image";

function MyButton() {
  return (
    <a 
      href="http://localhost:3000"
      target="_blank"
      rel = "noopener noreferrer"
      className = "px-4 py-2 bg-blue-500 text-white rounded-lg hover:bg-blue=600 transition duration=300"
    >
      Buka Halaman
    </a>
  )
}

export default function Home() {
  return (
    <div className="grid grid-rows-[20px_1fr_20px] items-center justify-items-center min-h-screen p-8 pb-20 gap-16 sm:p-20 font-[family-name:var(--font-geist-sans)]">
      <main className="flex flex-col gap-8 row-start-2 items-center sm:items-start">
        <Image
          className="dark:invert"
          src="/next.svg"
          alt="Next.js logo"
          width={180}
          height={38}
          priority
        />
        <ol className="list-inside list-decimal text-sm text-center sm:text-left font-[family-name:var(--font-geist-mono)]">
          <li className="mb-2">
            Get started by editing{" "}
            <code className="bg-black/[.05] dark:bg-white/[.06] px-1 py-0.5 rounded font-semibold">
              src/app/page.tsx
            </code>
            .
          </li>
          <li>Save and see your changes instantly.</li>
        </ol>

        <div className="flex gap-4 items-center flex-col sm:flex-row">
          <a
            className="rounded-full border border-solid border-transparent transition-colors flex items-center justify-center bg-foreground text-background gap-2 hover:bg-[#383838] dark:hover:bg-[#ccc] text-sm sm:text-base h-10 sm:h-12 px-4 sm:px-5"
            href="https://vercel.com/new?utm_source=create-next-app&utm_medium=appdir-template-tw&utm_campaign=create-next-app"
            target="_blank"
            rel="noopener noreferrer"
          >
            <Image
              className="dark:invert"
              src="/vercel.svg"
              alt="Vercel logomark"
              width={20}
              height={20}
            />
            Deploy now
          </a>
          <a
            className="rounded-full border border-solid border-black/[.08] dark:border-white/[.145] transition-colors flex items-center justify-center hover:bg-[#f2f2f2] dark:hover:bg-[#1a1a1a] hover:border-transparent text-sm sm:text-base h-10 sm:h-12 px-4 sm:px-5 sm:min-w-44"
            href="https://nextjs.org/docs?utm_source=create-next-app&utm_medium=appdir-template-tw&utm_campaign=create-next-app"
            target="_blank"
            rel="noopener noreferrer"
          >
            Read our docs
          </a>
          <MyButton />
        </div>
      </main>
      ...
    </div>
  );
}
~~~

![Result](public\img\p3-1_result.png)

### Jawaban Soal Praktikum 4
1. Untuk apakah kegunaan sintaks user.imageUrl? 

Sintaks tersebut digunakan untuk mendapatkan url dari nilai imageUrl yang ada pada variable user. dimana imageUrl adalah key dari atribut yang ada pada variable objek user

2. Buktikan dengan screenshoot yang menunjukkan bahwa tahapan percobaan di atas telah berhasil Anda lakukan!

Perubahan page.txt
~~~typescript
import Image from "next/image";

function MyButton() {
  return (
    <a 
      href="http://localhost:3000"
      target="_blank"
      rel = "noopener noreferrer"
      className = "px-4 py-2 bg-blue-500 text-white rounded-lg hover:bg-blue=600 transition duration=300"
    >
      Buka Halaman
    </a>
  );
}

function Profile() {
  return (
    <>
    <div className="text-xs">Develop by: {user.name}</div>
      <img 
        src={user.imageUrl}
        alt={'Foto' + user.name} 
        style={{
          width: user.imageSize,
          height: user.imageSize,
        }}
      />
    </>
  );
}

const user = {
  name: "Fulanah bin Fulan",
  imageUrl: "https://i.imgur.com/yXOvdOSs.jpeg",
  imageSize: 90,
}

export default function Home() {
  return (
    <div className="grid grid-rows-[20px_1fr_20px] items-center justify-items-center min-h-screen p-8 pb-20 gap-16 sm:p-20 font-[family-name:var(--font-geist-sans)]">
      <main className="flex flex-col gap-8 row-start-2 items-center sm:items-start">
        <Image
          className="dark:invert"
          src="/next.svg"
          alt="Next.js logo"
          width={180}
          height={38}
          priority
        />
        <ol className="list-inside list-decimal text-sm text-center sm:text-left font-[family-name:var(--font-geist-mono)]">
          <li className="mb-2">
            Get started by editing{" "}
            <code className="bg-black/[.05] dark:bg-white/[.06] px-1 py-0.5 rounded font-semibold">
              src/app/page.tsx
            </code>
            .
          </li>
          <li>Save and see your changes instantly.</li>
        </ol>

        <div className="flex gap-4 items-center flex-col sm:flex-row">
          <a
            className="rounded-full border border-solid border-transparent transition-colors flex items-center justify-center bg-foreground text-background gap-2 hover:bg-[#383838] dark:hover:bg-[#ccc] text-sm sm:text-base h-10 sm:h-12 px-4 sm:px-5"
            href="https://vercel.com/new?utm_source=create-next-app&utm_medium=appdir-template-tw&utm_campaign=create-next-app"
            target="_blank"
            rel="noopener noreferrer"
          >
            <Image
              className="dark:invert"
              src="/vercel.svg"
              alt="Vercel logomark"
              width={20}
              height={20}
            />
            Deploy now
          </a>
          <a
            className="rounded-full border border-solid border-black/[.08] dark:border-white/[.145] transition-colors flex items-center justify-center hover:bg-[#f2f2f2] dark:hover:bg-[#1a1a1a] hover:border-transparent text-sm sm:text-base h-10 sm:h-12 px-4 sm:px-5 sm:min-w-44"
            href="https://nextjs.org/docs?utm_source=create-next-app&utm_medium=appdir-template-tw&utm_campaign=create-next-app"
            target="_blank"
            rel="noopener noreferrer"
          >
            Read our docs
          </a>
          <MyButton />
        </div>
        <Profile />
      </main>
      ...
    </div>
  );
}
~~~

![Result](public\img\p4-2_result.png)
