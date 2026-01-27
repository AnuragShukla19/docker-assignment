# Startup Funding Tracker

A production-ready web application to track startup funding trends powered by Firecrawl API. Built with Next.js 14, TypeScript, and Tailwind CSS.

![Startup Funding Tracker](https://img.shields.io/badge/Next.js-14-black) ![TypeScript](https://img.shields.io/badge/TypeScript-5.3-blue) ![License](https://img.shields.io/badge/license-MIT-green)

## ✨ Features

- 🔍 **Real-time search** for startup funding data using Firecrawl API
- 📊 **Interactive trend charts** and comprehensive metrics dashboard
- 🎯 **Advanced filters** by time period (today, this week, this month)
- 🏷️ **Category filters** (AI, Fintech, HealthTech, and more)
- 💰 **Auto-extraction** of funding amounts, round types, and contact information
- 🌍 **Global coverage** of funding news from multiple sources
- 📈 **AI-powered insights** and funding trend summaries
- 💳 **API cost control** with configurable result limits (10/50/100 results)
- 🎨 **Beautiful UI** inspired by Firecrawl's design language
- ⚡ **Production-ready** with full TypeScript support and error handling

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ and npm
- Firecrawl API key ([Get one here](https://firecrawl.dev))

### Installation

1. **Clone and install dependencies:**
```bash
cd "c:\Users\Bhanu Partap\Downloads\FireCrawl"
npm install
```

2. **Set up environment variables:**
```bash
# Copy the example env file
cp .env.example .env.local

# Add your Firecrawl API key to .env.local
FIRECRAWL_API_KEY=fc-your-api-key-here
```

3. **Run the development server:**
```bash
npm run dev
```

4. **Open your browser:**
Navigate to [http://localhost:3000](http://localhost:3000)

## 🏗️ Build for Production

```bash
# Create optimized production build
npm run build

# Start production server
npm start
```

## 📋 Project Structure

```
FireCrawl/
├── app/
│   ├── api/
│   │   └── search/
│   │       └── route.ts          # Firecrawl API integration
│   ├── globals.css               # Global styles
│   ├── layout.tsx                # Root layout
│   └── page.tsx                  # Main page component
├── components/
│   ├── MetricsDisplay.tsx        # Trend metrics cards
│   ├── SearchBar.tsx             # Search and filter interface
│   ├── SummarySection.tsx        # Results and insights
│   └── TrendChart.tsx            # Interactive chart
├── types/
│   └── index.ts                  # TypeScript type definitions
├── .env.local                    # Environment variables (not in git)
├── .env.example                  # Example environment file
├── next.config.js                # Next.js configuration
├── tailwind.config.js            # Tailwind CSS configuration
├── tsconfig.json                 # TypeScript configuration
└── package.json                  # Dependencies
```

## 🎨 Design System

### Color Palette
- **Primary Orange**: `#f97316` - Main accent color (buttons, highlights)
- **Neutral Gray**: `#fafafa` - Background color
- **White**: `#ffffff` - Card backgrounds
- **Text Primary**: `#171717` - Main text
- **Text Secondary**: `#737373` - Secondary text

### Components
- Clean card-based layout with subtle shadows
- Orange CTA buttons with hover effects
- Responsive grid system
- Smooth transitions and animations

## 🔧 Configuration

### Result Limits
Control API costs by selecting result limits:
- **10 results** (2 credits) - Quick searches
- **50 results** (10 credits) - Medium datasets
- **100 results** (20 credits) - Comprehensive analysis

### Time Filters
- **Today** - Past 24 hours
- **This Week** - Past 7 days
- **This Month** - Past 30 days

### Categories
AI & Machine Learning, Finance & Fintech, Healthcare & Biotech, E-commerce & Retail, SaaS & Enterprise, Crypto & Web3, Climate & Clean Energy, Education Technology

## 🔍 How It Works

1. **User enters search query** with filters (category, time period, result limit)
2. **API constructs search query** combining user input with funding-related keywords
3. **Firecrawl API searches** web and news sources for relevant articles
4. **Content is scraped** and parsed to extract funding details:
   - Funding amounts ($5M, $2.5B, etc.)
   - Round types (Series A/B/C, Seed, Angel)
   - Company names and contact information
   - Website links
5. **Results are displayed** with metrics, charts, and detailed cards
6. **AI-generated insights** provide context and trends

## 📊 Data Extraction

The app uses advanced regex patterns to extract:
- **Funding Amounts**: `$5 million`, `$2.5B`, `raised $10M`
- **Round Types**: `Series A`, `seed round`, `pre-seed`
- **Email Addresses**: Standard email format validation
- **Company Names**: Extracted from article titles
- **Dates**: When funding was announced

## 🚀 Deployment

### Vercel (Recommended)

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

Add your `FIRECRAWL_API_KEY` in the Vercel dashboard under Environment Variables.

### Other Platforms
The app can be deployed to any Node.js hosting platform:
- Netlify
- Railway
- Render
- AWS Amplify
- DigitalOcean App Platform

## 🛡️ Production Features

✅ **TypeScript** - Full type safety across the application  
✅ **Error Handling** - Comprehensive error boundaries and user feedback  
✅ **Loading States** - Skeleton screens and loading indicators  
✅ **Responsive Design** - Mobile, tablet, and desktop optimized  
✅ **Environment Variables** - Secure API key management  
✅ **Build Optimization** - Code splitting and tree shaking  
✅ **SEO Ready** - Proper meta tags and semantic HTML  

## 📈 API Cost Optimization

- Configurable result limits to control API usage
- Clear credit cost display (2 credits per 10 results)
- Cached results to avoid redundant searches (coming soon)
- Efficient data extraction minimizes scraping needs

## 🐛 Troubleshooting

### Build Errors
```bash
# Clean build cache
rm -rf .next
npm run build
```

### Type Errors
```bash
# Check TypeScript errors
npx tsc --noEmit
```

### API Errors
- Verify your Firecrawl API key is correct
- Check API rate limits and credit balance
- Ensure internet connectivity

## 📝 License

MIT License - feel free to use this project for personal or commercial purposes.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 🔗 Links

- [Firecrawl Documentation](https://docs.firecrawl.dev)
- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com)

## 📞 Support

For issues or questions:
- Open an issue on GitHub
- Check Firecrawl documentation
- Review Next.js troubleshooting guide

---

Built with ❤️ using Firecrawl API
