# Sakthiiv's Personal Website

Personal website built with Hugo and Hugo Blox Builder, featuring academic CV, projects, publications, and teaching materials.

## 🚀 Quick Start

### Prerequisites

- **Go**: 1.19+ (currently using Go 1.24.5)
- **Hugo**: 0.149.0+ extended version
- **Node.js**: For TailwindCSS processing

### Installation

1. **Install Hugo Extended** (required for image processing):
   ```bash
   # Download latest Hugo Extended
   curl -L https://github.com/gohugoio/hugo/releases/latest/download/hugo_extended_$(curl -s https://api.github.com/repos/gohugoio/hugo/releases/latest | grep -o '"tag_name": "v[^"]*"' | cut -d'"' -f4)_darwin-universal.tar.gz | tar -xz
   ```

2. **Install Node.js dependencies**:
   ```bash
   npm install
   ```

### Development

1. **Start local server**:
   ```bash
   hugo server -D
   ```
   Site will be available at http://localhost:1313

2. **Build for production**:
   ```bash
   hugo --minify
   ```

## 🤝 Contributing

This is a personal website repository. For Hugo-related contributions, please contribute to the [Hugo project](https://github.com/gohugoio/hugo) instead.
