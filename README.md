# bioinf_hw1

# Сборка генома бактерии, выделенной из воды с нефтью, на основании парно-концевых (paired-end, PE) и чтений типа mate-pairs (MP).

Соержимое репозитория:

`data` - итоговые fasta файлы с последовательностями контигов и скаффолдов

`src` - ноутбук с кодом

`images` - полные результаты работы MultiQC

## Оценка качества чтений данных

Качество исходных чтений по результатам multiqc:

<img width="1551" height="324" alt="general" src="https://github.com/user-attachments/assets/639dc0f7-5a1b-473c-a462-be752d662719" />
<img width="1600" height="800" alt="fastqc_per_base_sequence_quality_plot" src="https://github.com/user-attachments/assets/7111dd35-48c1-4d37-a29e-c8929a681b1c" />


Качество после подрезания:

<img width="1546" height="311" alt="general_2" src="https://github.com/user-attachments/assets/43bd1b1a-16bf-45f7-ae66-f02e98f42ed4" />
<img width="1538" height="783" alt="Снимок экрана 2026-10-04 163908" src="https://github.com/user-attachments/assets/da4435db-9239-40b5-b212-23587515a449" />

Таким образом, видим, что подрезание сработало корректно и остались только чтения с хорошим качеством. Также можно отметить, что для paired-end чтений число отрезанных около 4%, в то время как для mate pair их число составляет порядка 40% от первоначального.


