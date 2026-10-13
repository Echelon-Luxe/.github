# LogiTrack

A microservices-based logistics and shipment-tracking platform deployed on AWS EKS and DigitalOcean Kubernetes. We’re implementing Docker containerization, CI/CD with GitHub Actions, GitOps with Argo CD, SAST, DAST, SonarQube-Cloud and container security scanning.
We can’t keep all services running due to cloud costs, so feel free to explore the repo or contribute.

<p align="center">
  <img src="assets/login-preview.png" alt="LogiTrack login screen" width="900">
</p>

## Services

| Service | Repo |
|---------|------|
| API gateway | [logitrack-api-gateway](https://github.com/Echelon-Luxe/logitrack-api-gateway) |
| Frontend | [logitrack-frontend](https://github.com/Echelon-Luxe/logitrack-frontend) |
| Users | [logitrack-user-service](https://github.com/Echelon-Luxe/logitrack-user-service) |
| Shipments | [logitrack-shipment-service](https://github.com/Echelon-Luxe/logitrack-shipment-service) |
| Drivers | [logitrack-driver-service](https://github.com/Echelon-Luxe/logitrack-driver-service) |
| Tracking | [logitrack-tracking-service](https://github.com/Echelon-Luxe/logitrack-tracking-service) |
| Notifications | [logitrack-notification-service](https://github.com/Echelon-Luxe/logitrack-notification-service) |
| Payments | [logitrack-payment-service](https://github.com/Echelon-Luxe/logitrack-payment-service) |

Everything routes through the API gateway; the backends stay cluster-internal. Deployment lives in [logitrack-infrastructure](https://github.com/Echelon-Luxe/logitrack-infrastructure) (Helm chart, cluster config, GitOps).
