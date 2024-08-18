# job-analysis

Ежедневно работодатели публикуют тысячи вакансий в самых разных сферах деятельности. Тот факт, что зарплата часто не указывается в тексте вакансии, усложняет процесс размещения вакансий для самих же работодателей, т.к. им в итоге сложно оценить обстановку на рынке и предоставить соискателям интересное предложение. При этом, если заработная плата указана, работодателям проще и рекомендовать вакансию заинтересованным людям, и подбирать подходящих кандидатов. 

Нашей задачей было составить модель, которая бы предсказывала заработную плату, которую может поставить работодатель, по параметрам вакансии

У нас был уже собраный датасет из которого мы взяли такие параметры, как график работы, опыт работы, регион(где предоставляется вакансия), специальность и описание вакансии. На нем мы протестировали модели линейная регрессия, дерево решений и случайный лес решений. Самой подходящей оказалась модель линейная регрессия. Для оценки мы использовали метрики mse, r2 и mape, соответствующие результаты: 15406, 0.46 и 0.35

Так же мы скачали данные с сайта hh.ru, чтобы было больше данных для обработки. Однако там не оказалось параметра "описание вакансии", поэтому мы отдельно тестировали те же модели, но для уже соединенных баз данных(без описания вакансии).Лучшей оказалась модель дерево решений. Для оценки использовали те же метрики mse, r2 и mape, соответствующие результаты: 17995, 0.22, 0.35

ссылка на данные https://drive.google.com/drive/folders/1UYskqoaFwP8z_hc3L08QSjQSjb8dXNMu?usp=sharing
