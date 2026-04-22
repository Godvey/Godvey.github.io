# Academic Pages (L-ORE Lab Optimized Edition)

[![GitHub stars](https://img.shields.io/github/stars/Godvey/godvey.github.io?style=flat-square)](https://github.com/Godvey/godvey.github.io/stargazers)
[![GitHub license](https://img.shields.io/github/license/Godvey/godvey.github.io?color=blue&style=flat-square)](https://github.com/Godvey/godvey.github.io/blob/master/LICENSE)

This is an optimized version of the [Academic Pages](https://academicpages.github.io/) template, specifically customized for **Robotics, Engineering, and UAV Swarm Research Labs**. 

Developed and maintained by **Wei Yu (L-ORE Lab, City University of Macau)**.

---

## 🚀 Enhancements in this Edition

Compared to the vanilla Academic Pages, this version includes several "hard-coded" improvements for research group visibility:

1.  **Three-Column Member Layout**: A specialized CSS/HTML structure for displaying large research teams (Ph.D., Master, and Undergraduate) in a clean, side-by-side grid.
2.  **Built-in Recruitment System**: Pre-configured "Apply" buttons and recruitment status indicators to help labs attract prospective students.
3.  **Research Infrastructure Showcase**: A dedicated grid layout for showcasing lab equipment, flight arenas, and hardware platforms.
4.  **Professional Academic Footer**: Removed redundant "Site last updated" timestamps and streamlined copyright information for a cleaner academic look.
5.  **Mobile-Optimized UI**: Enhanced touch-target sizes for "Apply" buttons and responsive member cards for mobile viewing.

---

## 🛠️ Getting Started

### 1. Repository Setup
1.  Click the **"Use this template"** button in the top right to create your own copy.
2.  Name the repository `[your-github-username].github.io`.
3.  Edit `_config.yml` to update your `url`, `baseurl`, and personal information.

### 2. Customizing the Portfolio Page
The specialized lab layout is located in `_pages/portfolio.md` (or your chosen permalink page). You can directly copy the `<style>` block and HTML structure to manage your lab members and infrastructure.

### 3. Local Development
To preview changes locally, you need Ruby and Jekyll:
```bash
bundle install
bundle exec jekyll serve -l -H localhost
