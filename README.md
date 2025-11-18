# Hire Gem - AI-Powered Profile Analyzer

## About the Project

Hire Gem is an intelligent profile analysis platform that helps recruiters and hiring managers make data-driven decisions by comprehensively analyzing candidate profiles. The system extracts information from CVs, scrapes data from professional platforms like GitHub, LinkedIn, DevPost, and Kaggle, and provides detailed insights including match scores, strengths, weaknesses, and personalized recommendations.

## What Inspired You

The inspiration came from the challenge of manually reviewing hundreds of resumes and cross-referencing candidate information across multiple platforms. Traditional hiring processes are time-consuming and often miss critical information buried in online portfolios or project repositories. We wanted to create a solution that automates this process while providing deeper insights through AI-powered analysis.

## What You Learned

Building Hire Gem taught us several valuable lessons. We learned how to integrate multiple APIs and web scraping tools effectively, including Firecrawl for reliable content extraction and Google's Gemini AI for intelligent analysis. We discovered the complexities of parsing different document formats (PDF, DOCX, TXT) and extracting meaningful data. Most importantly, we learned how to build an AI agent system that can iteratively use multiple tools to answer complex questions, making the system truly intelligent rather than just automated.

## How You Built Your Project

The project was built using Flask as the backend framework, providing a clean REST API structure. We integrated Google Gemini 2.5 Flash for AI-powered analysis and Firecrawl for web scraping capabilities. The frontend was designed with a modern, minimalistic UI using vanilla JavaScript for dynamic interactions. 

The core workflow involves: extracting text from uploaded CVs, scraping profile data from various platforms, using AI to generate comprehensive analyses, and storing everything in an organized file system. The AI agent chat feature uses an iterative tool-calling system where the agent can use multiple tools in sequence - looking up resume data, searching websites, and analyzing media - to provide accurate answers to user queries.

## Challenges You Faced

One of the biggest challenges was handling different document formats and extracting clean text from PDFs and DOCX files. We also faced difficulties with web scraping reliability, which led us to integrate Firecrawl for more consistent results. Building the AI agent with iterative tool usage required careful prompt engineering to ensure the agent makes intelligent decisions about when and how to use each tool. Another challenge was managing token limits when processing large amounts of data while still providing comprehensive analysis.

## Technical Stack

- Backend: Flask, Python
- AI: Google Gemini 2.5 Flash
- Web Scraping: Firecrawl, BeautifulSoup
- Document Processing: PyPDF2, python-docx
- Frontend: HTML, CSS, JavaScript
- Data Storage: File system with JSON structure
