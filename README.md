# SudoSelf - Professor Teece Digital Twin

A comprehensive digital twin application representing Professor David J. Teece's intellectual contributions across multiple domains of economics, business strategy, and innovation.

## Overview

This project implements a sophisticated AI system that captures Professor Teece's ideas, perspectives, and intellectual frameworks. It's designed to explain his theories on dynamic capabilities, innovation, and firm strategy while maintaining contextual awareness in conversations.

## Features

- Document Processing Pipeline with advanced document analysis
- Knowledge Extraction and Concept Mapping
- Multi-modal Response Generation
- Knowledge Graph Representation
- Temporal Context Analysis
- Jupyter Notebook Analysis (for document processing quality evaluation)

## Technical Architecture

The system is built on AWS cloud infrastructure:

- **Document Processing**: Lambda functions for document ingestion and analysis
- **Knowledge Storage**: DynamoDB, S3, and Neptune graph database
- **Embeddings**: SageMaker for vector representations
- **Response Generation**: AWS Bedrock for LLM-powered responses
- **Monitoring**: CloudWatch for system observability

## Documentation

For detailed information about specific features, see the documentation in the `docs/` directory.

## Jupyter Notebook Analysis

The Jupyter Notebook Analysis feature automatically generates analytical notebooks for each processed document. These notebooks provide statistical analysis, visualizations, and quality metrics to help evaluate document processing quality. See `features/notebook_analysis/` for implementation details.