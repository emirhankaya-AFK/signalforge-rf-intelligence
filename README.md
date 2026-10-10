# SignalForge

## English
### Purpose
RF spectrum intelligence and signal anomaly platform for electrical engineering applications.

### Verified Features
- FastAPI backend with RF device models, capture management, and spectrum analysis
- React TypeScript Vite frontend with dark RF-console UI and visualizations
- Deterministic synthetic IQ-signal generator for BPSK, QPSK, 16QAM, and FM-like modulations
- DSP features including FFT PSD, spectral centroid, bandwidth, and SNR estimation
- CPU-only scikit-learn modulation classifier and anomaly scoring
- REST endpoints and WebSocket spectrum feed
- Docker Compose, Kubernetes manifests, and CI/CD pipelines

### Stack
- Backend: FastAPI (Python)
- Frontend: React, TypeScript, Vite
- Containerization: Docker, Docker Compose
- Orchestration: Kubernetes (manifests provided)
- ML: scikit-learn (CPU-only)
- CI/CD: pipelines (as referenced)

### Setup & Usage
#### Prerequisites
- Docker and Docker Compose
- (Optional) Kubernetes cluster for production deployment

#### Local Development
1. Clone the repository
2. Copy `.env.example` to `.env` and adjust as needed
3. Run `make up` to start all services
4. Backend API available at http://localhost:8000
5. Frontend UI available at http://localhost:3000

#### Sample Data Generation
```bash
docker-compose run --rm backend python /app/scripts/generate_sample_data.py
```

### Limitations
- Modality classification is CPU-only (no GPU acceleration)
- Intended for local development via Docker Compose; production deployment assumes a Kubernetes cluster
- Synthetic data generation is for demonstration purposes

### License
MIT License – see [LICENSE](LICENSE) file for details.

## Türkçe
### Amaç
Elektrik mühendisliği uygulamaları için RF spektrumu zekası ve sinyal anomali platformu.

### Doğrulanmış Özellikler
- RF cihaz modelleri, yakalama yönetimi ve spektrum analizi için FastAPI backend'i
- Koyu RF-konsol UI ve görselleştirmeleri olan React TypeScript Vite frontend'i
- BPSK, QPSK, 16QAM ve FM benzeri modülasyonlar için deterministik sentetik IQ-sinyal üreteci
- FFT PSD, spektral centroid, bant genişliği ve SNR tahmini gibi DSP özellikleri
- CPU-only scikit-learn modülasyon sınıflandırıcı ve anomali puanı
- REST endpoint'leri ve WebSocket spektrum akışı
- Docker Compose, Kubernetes manifestleri ve CI/CD hatları

### Teknoloji Yığını
- Backend: FastAPI (Python)
- Frontend: React, TypeScript, Vite
- Konteynerleştirme: Docker, Docker Compose
- Orkestrasyon: Kubernetes (sağlanan manifestler)
- Makine öğrenimi: scikit-learn (sadece CPU)
- CI/CD: referanslanan hatlar

### Kurulum & Kullanım
#### Ön Koşullar
- Docker ve Docker Compose
- (Opsiyonel) Üretim dağıtımı için Kubernetes kümesi

#### Yerel Geliştirme
1. Depoyu klonlayın
2. `.env.example` dosyasını `.env` olarak kopyalayın ve gerektiği şekilde ayarlayın
3. `make up` komutunu çalıştırarak tüm hizmetleri başlatın
4. Backend API http://localhost:8000 adresinde kullanılabilir
5. Frontend UI http://localhost:3000 adresinde kullanılabilir

#### Örnek Veri Üretimi
```bash
docker-compose run --rm backend python /app/scripts/generate_sample_data.py
```

### Sınırlamalar
- Sınıflandırma sadece CPU üzerinde çalışır (GPU desteği yok)
- Yerel geliştirme Docker Compose ile; üretim dağıtımı Kubernetes kümesi gerektirir
- Sentetik veri üretimi sadece gösterim amaçlıdır

### Lisans
MIT Lisansı – [LICENSE](LICENSE) dosyasına bakın.

## Deutsch
### Zweck
RF-Spektrumsintelligenz und Signal-Anomalie-Plattform für elektrotechnische Anwendungen.

### Verifizierte Funktionen
- FastAPI-Backend mit RF-Gerätemodellen, Erfassung management und Spektrumanalyse
- React TypeScript Vite Frontend mit dunklem RF-Konsol-UI und Visualisierungen
- Deterministischer synthetischer IQ-Signalgenerator für BPSK, QPSK, 16QAM und FM-ähnliche Modulationen
- DSP-Funktionen einschließlich FFT-PSD, spektralem Schwerpunkt, Bandbreite und SNR-Schätzung
- CPU-only scikit-learn Modulationsklassifikator und Anomalienbewertung
- REST-Endpunkte und WebSocket-Spektrum-Feed
- Docker Compose, Kubernetes-Manifeste und CI/CD-Pipelines

### Technologie-Stack
- Backend: FastAPI (Python)
- Frontend: React, TypeScript, Vite
- Containerisierung: Docker, Docker Compose
- Orchestrierung: Kubernetes (bereitgestellte Manifeste)
- Maschinelles Lernen: scikit-learn (nur CPU)
- CI/CD: referenzierte Pipelines

### Einrichtung & Nutzung
#### Voraussetzungen
- Docker und Docker Compose
- (Optional) Kubernetes-Cluster für Produktionsbetrieb

#### Lokale Entwicklung
1. Repository klonen
2. `.env.example` nach `.env` kopieren und bei Bedarf anpassen
3. `make up` ausführen, um alle Dienste zu starten
4. Backend-API unter http://localhost:8000 erreichbar
5. Frontend-UI unter http://localhost:3000 erreichbar

#### Beispiel-Datengenerierung
```bash
docker-compose run --rm backend python /app/scripts/generate_sample_data.py
```

### Einschränkungen
- Die Klassifizierung erfolgt ausschließlich CPU-basiert (keine GPU-Beschleunigung)
- Lokale Entwicklung setzt Docker Compose voraus; Produktionsbetrieb setzt einen Kubernetes-Cluster voraus
- Synthetische Datengenerierung dient ausschließlich Demonstrationszwecken

### Lizenz
MIT-Lizenz – siehe [LICENSE](LICENSE) Datei für Details.
