# SignalForge

RF spectrum intelligence and signal anomaly platform for electrical engineering applications.

## Overview
SignalForge is a polished platform for RF spectrum intelligence and signal anomaly detection. It features:
- FastAPI backend with RF device models, capture management, and spectrum analysis
- React TypeScript Vite frontend with dark RF-console UI and visualizations
- Deterministic synthetic IQ-signal generator for BPSK, QPSK, 16QAM, and FM-like modulations
- DSP features including FFT PSD, spectral centroid, bandwidth, and SNR estimation
- CPU-only scikit-learn modulation classifier and anomaly scoring
- REST endpoints and WebSocket spectrum feed
- Docker Compose, Kubernetes manifests, and CI/CD pipelines

## Architecture
See [docs/architecture.md](docs/architecture.md) for detailed architecture.

## API Reference
See [docs/api.md](docs/api.md) for API documentation.

## Threat Model
See [docs/threat-model.md](docs/threat-model.md) for security considerations.

## Getting Started

### Prerequisites
- Docker and Docker Compose
- (Optional) Kubernetes cluster for production deployment

### Local Development
1. Clone the repository
2. Copy `.env.example` to `.env` and adjust as needed
3. Run `make up` to start all services
4. Backend API will be available at http://localhost:8000
5. Frontend UI will be available at http://localhost:3000

### Sample Data Generation
To generate sample data for demonstration:
```bash
docker-compose run --rm backend python /app/scripts/generate_sample_data.py
```

## License
MIT License - see [LICENSE](LICENSE) file for details.

## Documentation
- [Architecture](docs/architecture.md)
- [API Reference](docs/api.md)
- [Threat Model](docs/threat-model.md)