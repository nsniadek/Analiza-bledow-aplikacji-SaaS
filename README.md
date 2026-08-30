**Analiza błędów aplikacji SaaS — Power BI Dashboard**

📊 Business Intelligence | Power BI | Data Analysis

Dashboard analizujący błędy aplikacji SaaS pod kątem ich częstotliwości, czasu rozwiązania oraz wpływu na utratę klientów.


<img width="1446" height="810" alt="image" src="https://github.com/user-attachments/assets/0bbf2864-1c33-4710-adc2-f5cc30b3dc41" />





**🎯 Cel biznesowy**

Projekt odpowiada na pytania:

- Które moduły i typy błędów mają największy wpływ na odejście klientów w ciągu 30 dni od ich wystąpienia? 
- Jakie typy błędów występują najczęściej?
- Czy konkretne wersje aplikacji generują więcej problemów?
- Które segmenty klientów mają najdłuższy czas rozwiązania problemów?
- Czy średni czas rozwiązania incydentów o krytyczności Critical i High spełnia wymagania SLA dla klientów z segmentu Enterprise w porównaniu do pozostałych segmentów?
- Czy błędy o wysokiej krytyczności skupiają się na konkretnych systemach operacyjnych lub urządzeniach (np. Android vs iOS, Desktop vs Mobile)? 


**📌 Najważniejsze wnioski**

Na podstawie analizy zidentyfikowano kilka kluczowych obszarów:
- Płatności mają najwyższy wskaźnik rezygnacji klientów po wystąpieniu błędu — **23%**.
- Timeouty są najczęstszym typem błędu — **229 przypadków**.
- **Wersja 3.4** charakteryzuje się wyraźnie podwyższoną liczbą błędów.
- **Segment SMB** ma najdłuższy średni czas rozwiązania błędów krytycznych.
- Odsetek rozwiązanych błędów wynosi **89,1%**, czyli nieznacznie poniżej założonego celu >90%.
- Ogólny churn klientów po wystąpieniu błędu pozostaje poniżej założonego limitu, jednak moduł płatności stanowi istotny wyjątek.



**💡 Rekomendacje biznesowe**

Na podstawie wyników rekomendowane są:
1. Priorytetyzacja stabilności modułu płatności, ze względu na jego wpływ na churn.
2. Analiza źródeł timeoutów, szczególnie w kontekście API i wydajności aplikacji.
3. Szczegółowa analiza błędów w wersji 3.4.
4. Przegląd procesu obsługi krytycznych błędów dla segmentu SMB.


**🛠️ Wykorzystane narzędzia**
- Power BI
- DAX
- Power Query
- Data visualization
- Business analysis


**📈 Elementy dashboardu**
- KPI cards
- Segment filters
- Date filtering
- Error analysis by application module
- Error analysis by severity
- Resolution time analysis
- Customer churn analysis
- Error analysis by application version
- Operating system and device analysis


**📁 Struktura projektu**
dashboard/    → Power BI report

screenshots/  → dashboard preview

data/         → dataset used in the analysis


Note: The dataset is fictional/synthetic and is used solely for portfolio purposes.
