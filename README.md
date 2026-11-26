# AdCraftor – AI-Powered CGI Advertisement Video Generator



AdCraftor is a web application designed to simplify product advertising by turning product images into cinematic CGI advertisement videos through an AI-powered workflow.



## Overview



Traditional product advertising often requires photography studios, models, equipment, and video editing. AdCraftor aims to simplify this process by allowing users to upload a product image, customize model characteristics, and create advertisement content.



## Features



\- \*\*AI Model Generation:\*\* Customize model characteristics such as gender, body type, hair, skin tone, and pose.

\- \*\*Single Image Input:\*\* Upload a product photograph as the starting point for an advertisement.

\- \*\*Fast Ad Creation:\*\* Designed to reduce the time and effort required for traditional ad production.

\- \*\*Advertisement Variations:\*\* Explore different model and pose combinations.

\- \*\*CGI Video Generation:\*\* Designed to generate cinematic product advertisement videos.

\- \*\*Social Media Formats:\*\* Supports advertising use cases for platforms such as Instagram, Facebook, TikTok, and YouTube Shorts.

\- \*\*User Authentication:\*\* Sign up and sign in using email and password or Google.

\- \*\*Password Recovery:\*\* Request a password reset link.

\- \*\*Contact Form:\*\* Submit messages through the contact section.



## Technology Stack



| Category | Technologies |

|---|---|

| Frontend | React 18, TypeScript |

| Build Tool | Vite |

| Styling | Tailwind CSS |

| UI Components | shadcn/ui, Radix UI |

| Icons | Lucide React |

| Routing | React Router |

| Backend Services | Supabase |

| Authentication | Supabase Auth, Lovable OAuth integration |

| Database | Supabase / PostgreSQL |

| File Storage | Supabase Storage |

| Testing | Vitest, Playwright |



## Project Structure



```text

AdCraftor/

├── public/                  # Static assets

├── src/

│   ├── components/          # Reusable UI components

│   │   ├── landing/         # Landing page sections

│   │   └── ui/              # UI components

│   ├── hooks/               # Custom React hooks

│   ├── integrations/        # Supabase and service integrations

│   ├── pages/               # Application pages

│   └── ...

├── supabase/

│   ├── migrations/          # Database and storage migrations

│   └── config.toml          # Supabase configuration

├── package.json

├── vite.config.ts

└── README.md

```



## Getting Started



### Prerequisites



\- Node.js (LTS version recommended)

\- npm

\- A Supabase project



### 1. Clone the repository



```bash

git clone https://github.com/akshitabachhav/AdCraftor.git

```



### 2. Open the project directory



```bash

cd AdCraftor

```



### 3. Install dependencies



```bash

npm install

```



### 4. Configure environment variables



Create a `.env` file in the project root and add your Supabase project credentials:



```env

VITE\\\_SUPABASE\\\_URL=your\\\_supabase\\\_project\\\_url

VITE\\\_SUPABASE\\\_PUBLISHABLE\\\_KEY=your\\\_supabase\\\_publishable\\\_key

```



Replace the placeholder values with your actual Supabase project values.



\*\*Never commit your `.env` file or expose secret keys in the repository.\*\*



### 5. Configure Supabase



The repository includes SQL migration files in `supabase/migrations/`.



Apply the migrations to your Supabase project in chronological order. They define:



\- A `product-images` storage bucket.

\- A `generated-videos` storage bucket.

\- A `contact\\\_messages` database table.

\- Related storage and database access policies.



Configure Google authentication in Supabase if you want to use Google sign-in.



### 6. Start the development server



```bash

npm run dev

```



Open the local URL displayed in your terminal to view the application.



## Available Scripts



| Command | Description |

|---|---|

| `npm run dev` | Start the development server |

| `npm run build` | Build the production application |

| `npm run build:dev` | Build using development mode |

| `npm run preview` | Preview the production build |

| `npm run lint` | Run ESLint |

| `npm run test` | Run tests |

| `npm run test:watch` | Run tests in watch mode |



## Database and Storage



AdCraftor uses Supabase for backend services.



The included migrations configure:



\- \*\*product-images:\*\* Storage for uploaded product images.

\- \*\*generated-videos:\*\* Storage for generated video files.

\- \*\*contact\_messages:\*\* Stores contact form submissions, including name, email, message, and submission timestamp.



\*\*Security note:\*\* The supplied migrations define public read and upload policies for the two storage buckets and allow anonymous or authenticated users to submit contact messages. Review and strengthen these policies before using the application with real customer data or in production.



## Future Scope



Potential areas for further development include:



\- Complete AI-powered video generation workflow.

\- Additional model customization options.

\- More advertisement templates and aspect ratios.

\- Video preview and download functionality.

\- Improved access controls and storage security.

\- Production deployment and performance optimization.



## Original Project Credits



This repository contains the AdCraftor academic project. Please retain appropriate credit for the original project contributors:



\- Pranav Jadhav

\- Akshita Bachhav

\- Krushna Shirsath

\- Ganesh Tare



\*\*Project Guide:\*\* Prof. (Dr.) N. R. Wankhade



\*\*Institution:\*\* Late G. N. Sapkal College of Engineering, Anjaneri, Nashik.



## License



No license has been specified for this repository. Please obtain the original contributors' permission and add an appropriate license before allowing reuse or redistribution.

