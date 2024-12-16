
# 🛠 **리뷰 분석 및 시각화 서비스**

---

## 📌 **서비스 개요**  
이 서비스는 **Google Sheets**에 저장된 **2000개의 배달의민족 리뷰 데이터**를 기반으로,  
다양한 **분석 및 시각화** 기능을 제공하는 **AI 기반 리뷰 분석 시스템**입니다.

---

## 🚀 **주요 기능**  

### **리뷰 분석**  
- **GPT API**를 활용해 매장의 리뷰 데이터를 분석합니다.  
- **메뉴**에서 가장 많이 언급된 메뉴 **1위와 2위**를 도출합니다.  
- 리뷰 내용을 바탕으로 매장의 **강점**과 **약점**을 추출합니다.  
- 모든 리뷰를 요약하여 **한 줄로 요약된 결과**를 제공합니다.  

### **리뷰 시각화**  
- **Word Cloud API**를 활용해 리뷰에서 많이 언급된 **단어의 빈도수**를 추출하고 시각화합니다.  
- 긍정적 리뷰(별점 4 이상)와 부정적 리뷰(별점 3 이하)를 나누어 **워드클라우드**로 보여줍니다.  

---

## 🚀 **서비스 흐름**  

### **1. 데이터 입력**  
- Google Sheets에 저장된 **2000개 리뷰 데이터**를 불러옵니다.  
- 리뷰 데이터에는 다음 정보가 포함됩니다:  
   - **`rating`**: 별점  
   - **`content`**: 리뷰 내용  
   - **`menu`**: 메뉴 이름  

### **2. 데이터 분석**  
- **GPT API**를 통해 다음 분석을 수행합니다:  
   - 메뉴 중 **가장 많이 언급된 메뉴 1위와 2위** 도출  
   - 리뷰 내용을 기반으로 **강점과 약점** 분석  
   - 모든 리뷰를 **한 문장으로 요약**  

### **3. 시각화**  
- **Word Cloud API**를 활용해 리뷰의 단어 빈도를 시각화합니다:  
   - 긍정적 리뷰(별점 4 이상)와 부정적 리뷰(별점 3 이하)를 분리하여 시각화  
   - 많이 언급된 단어들을 **워드클라우드 이미지**로 출력  

---

## 📊 **분석 데이터 예시**  

### **상위 메뉴 분석**  
- **1위 메뉴**: [딸기맛] 생과일 화채 정식빙수  
- **2위 메뉴**: 수박 가득하게 화채빙수  

### **리뷰 요약**  
> 이 매장의 과일 디저트는 대체로 신선하고 맛있으며, 양이 많아 만족감을 제공하지만 한 건의 낮은 평가는 주스의 품질에 대한 불만을 제기하고 있습니다.

### **강점**  
1. 과일의 신선함  
2. 풍성한 양  
3. 다양한 서비스 제공  

### **약점**  
1. 주스 품질에 대한 일부 불만  
2. 과일 당도 변동  
3. 특정 제품의 높은 가격  

---

## 🚀 **서비스 워크플로우**  

아래 이미지는 전체 **워크플로우**를 시각화한 모습입니다:

### **워크플로우 이미지**  
<img width="836" alt="스크린샷 2024-12-17 오전 1 46 54" src="https://github.com/user-attachments/assets/178d3eb9-4369-47ba-9a13-a60a2b63cb33" />


---

## 🛠 **기술 스택**  

| **구분**         | **사용 기술**                 | **설명**                               |  
|------------------|-------------------------------|---------------------------------------|  
| **데이터 저장**   | Google Sheets                | 리뷰 데이터 저장 및 필터링             |  
| **AI 분석**      | OpenAI GPT API               | 리뷰 분석 및 요약                     |  
| **시각화**       | QuickChart Word Cloud API    | 단어 빈도 기반 시각화 생성             |  
| **자동화**       | n8n                          | 데이터 흐름 및 서비스 자동화 관리      |  

---

## 📷 **결과 시각화 예시**  

### **긍정적 워드클라우드**  
![wordcloud (2)](https://github.com/user-attachments/assets/9241038c-80aa-467e-bdc3-f01c45fc36b4)

---

## 🔗 **결론**  

이 서비스는 **AI와 시각화 기술**을 활용해 **리뷰 데이터를 효과적으로 분석**하고 인사이트를 제공합니다.  
데이터 기반의 평가와 시각화는 음식점 운영자와 소비자 모두에게 유용한 정보를 제공합니다.
