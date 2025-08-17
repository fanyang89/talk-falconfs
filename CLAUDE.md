# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Slidev presentation project for a technical talk about FalconFS, a distributed file system designed for large-scale deep learning pipelines. The presentation is in Chinese and covers the architecture, challenges, and performance benefits of FalconFS compared to traditional distributed file systems like CephFS and Lustre.

## Development Commands

- `pnpm install` - Install dependencies
- `pnpm dev` - Start development server with hot reload (opens http://localhost:3030)
- `pnpm build` - Build the presentation for production
- `pnpm export` - Export the presentation to static files

## Project Structure

- `slides.md` - Main presentation content in Chinese, covering FalconFS architecture and deep learning storage challenges
- `components/` - Vue components used in slides
  - `Counter.vue` - Interactive counter component with increment/decrement buttons
- `pages/` - Additional slide content that can be imported
- `snippets/` - TypeScript code snippets that can be embedded in slides
  - `external.ts` - Utility functions and example code
- `public/` - Static assets including images referenced in slides
- `netlify.toml` - Netlify deployment configuration
- `vercel.json` - Vercel deployment configuration

## Slidev Configuration

The presentation uses:
- Theme: `apple-basic` with custom Chinese fonts (方正屏显雅宋_GBK)
- Features: MDC syntax support, drawings, custom transitions
- Layouts: Custom layouts including intro-image and intro-image-right

## Key Technical Topics Covered

The presentation discusses:
- Deep learning workload patterns (billions of small files, random access)
- POSIX I/O limitations in distributed environments
- Client-side metadata caching issues
- FalconFS's stateless client architecture
- Hybrid metadata indexing approach
- Lazy namespace replication
- Performance comparisons with CephFS and Lustre

## Deployment

The project is configured for deployment on both Netlify and Vercel platforms with proper build settings and routing configurations.