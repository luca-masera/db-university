1. Contare quanti iscritti ci sono stati ogni anno

2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio
SELECT COUNT(*) AS `numero_insegnanti`,`office_address`FROM `teachers`GROUP BY `office_address`;

3. Calcolare la media dei voti di ogni appello d'esame
SELECT AVG(`vote`) AS 'media dei voti' FROM `exam_student`;
SELECT AVG(`vote`) AS 'media voti' FROM `exam_student` GROUP BY 'media voti';


4. Contare quanti corsi di laurea ci sono per ogni dipartimento
SELECT COUNT(`id`) AS `num_corsi`, `department_id` AS `num_dipartimento`
FROM `degrees` 
GROUP BY `department_id`;