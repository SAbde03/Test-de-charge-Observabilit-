<img width="1858" height="819" alt="Screenshot 2026-01-02 001749" src="https://github.com/user-attachments/assets/ae2bdba5-e5a3-4f0c-9450-7e9eef121b7f" />
<img width="1867" height="865" alt="Screenshot 2026-01-02 001811" src="https://github.com/user-attachments/assets/509ac38c-4a51-4a6e-91ca-910a339f22d7" />
<img width="1856" height="819" alt="Screenshot 2026-01-02 001929" src="https://github.com/user-attachments/assets/44d3a409-fbc5-41ab-b6aa-02c18a03e6c4" />
<img width="659" height="337" alt="Screenshot 2026-01-02 002846" src="https://github.com/user-attachments/assets/a24dae3f-5b28-4b5c-b7ee-38cc2c758ca9" />
<img width="974" height="208" alt="Screenshot 2026-01-02 003311" src="https://github.com/user-attachments/assets/0310881b-1e65-4fed-9290-54518c2821e1" />
<img width="1859" height="817" alt="Screenshot 2026-01-02 003510" src="https://github.com/user-attachments/assets/a1771295-7284-438d-bb64-ffd404efe967" />
<img width="1859" height="867" alt="Screenshot 2026-01-02 003638" src="https://github.com/user-attachments/assets/c194ba81-d724-454b-ba4d-668c29f5097a" />
<img width="658" height="274" alt="Screenshot 2026-01-02 003801" src="https://github.com/user-attachments/assets/c09b453c-eea5-4125-86f3-0e1865e64725" />

## Conclusion
Le verrou DB est important en architecture multi-instances pour garantir la cohérence des données lors d'accès concurrents : il force MySQL à traiter les requêtes une par une sur une ressource partagée, empêchant ainsi plusieurs conteneurs de décrémenter un stock simultanément et d'aboutir à des valeurs incohérentes ou négatives. En complément, le Circuit Breaker assure la résilience du système en isolant un service défaillant pour éviter la propagation des pannes en cascade, tandis que le Fallback fournit une réponse de secours "dégradée" afin de maintenir la continuité du service pour l'utilisateur final malgré l'erreur.
