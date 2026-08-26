# 🧬 AI Molecular Design Platform

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.95+-green.svg)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/React-18.0+-blue.svg)](https://reactjs.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-orange.svg)](https://pytorch.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Gemini](https://img.shields.io/badge/Gemini-AI-purple.svg)](https://deepmind.google/technologies/gemini/)
[![PRs](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![GitHub stars](https://img.shields.io/github/stars/yourusername/AI-Molecular-Design-Platform)](https://github.com/yourusername/AI-Molecular-Design-Platform/stargazers)

---

## 🌟 Overview

**AI Molecular Design Platform** is an end-to-end artificial intelligence system that revolutionizes molecular discovery by generating novel molecules with desired properties and optimizing existing ones using state-of-the-art deep learning techniques.

> 🎯 **Mission**: Accelerate drug discovery and materials science through intelligent, autonomous molecular design.

### 🔬 Key Capabilities

| Capability | Technology | Description |
|------------|------------|-------------|
| **Molecule Generation** | Diffusion Models | Create novel 3D molecules conditioned on target properties |
| **Property Prediction** | Graph Neural Networks | Predict molecular properties with high accuracy |
| **Molecule Optimization** | Reinforcement Learning | Optimize molecules for specific properties iteratively |
| **AI Assistance** | Gemini API | Get intelligent suggestions and scientific explanations |
| **Interactive Visualization** | 3Dmol.js | View and interact with molecules in 3D space |

---

## 🎯 Core AI Technologies

### 1. 🧠 Graph Neural Networks (GNN)
- **Purpose**: Predict molecular properties from molecular graphs
- **Architecture**: Equivariant GNN with attention-based pooling
- **Features**: 
  - Atom-level feature extraction
  - Edge-based message passing
  - 3D geometry awareness
- **Prediction Targets**: Binding affinity, drug-likeness, solubility, ADMET properties

### 2. 🔄 Diffusion Models
- **Purpose**: Generate novel molecules from scratch
- **Architecture**: SE(3)-equivariant diffusion with 3D awareness
- **Features**:
  - Conditional generation based on target properties
  - 20× faster sampling optimization
  - Semi-flexible molecular generation
- **Generation Process**: Noise → Denoising → Valid 3D molecule

### 3. 🎯 Reinforcement Learning Agent
- **Purpose**: Optimize molecules for specific properties
- **Algorithm**: Proximal Policy Optimization (PPO)
- **Features**:
  - Multi-objective optimization
  - Continuous learning loop
  - Reward-driven refinement
- **Optimization Goals**: Potency, selectivity, stability, synthesizability

### 4. 🤖 Gemini AI Integration
- **Purpose**: Provide intelligent molecular design assistance
- **Capabilities**:
  - Natural language queries
  - Property suggestions
  - Scientific explanations
  - Alternative design proposals

---

## 🏗️ System Architecture



---

## 🚀 Quick Start Guide

### Prerequisites

| Requirement | Version | Check |
|-------------|---------|-------|
| Python | 3.9+ | `python --version` |
| Node.js | 16+ | `node --version` |
| npm | 8+ | `npm --version` |
| Git | Latest | `git --version` |
| Gemini API Key | - | Get from Google AI Studio |

### Installation

#### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/AI-Molecular-Design-Platform.git
cd AI-Molecular-Design-Platform

# Navigate to backend directory
cd backend

# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env and add your GEMINI_API_KEY

# Run backend server
python run.py


# Navigate to frontend directory
cd frontend

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env and add your API URL

# Run frontend development server
npm run dev