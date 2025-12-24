---
title: Untitled Page
description: 
published: true
date: 2025-12-24T10:13:21.200Z
tags: 
editor: markdown
dateCreated: 2025-12-24T10:13:21.200Z
---

# Сущности схемы `mart_sv`

*Обновлено: 2025-12-24 10:08*
*Всего сущностей: 358*

| Название | Тип | Описание |
|----------|-----|----------|
| `a_b_test_lezhaki` | BASE TABLE |  |
| `ab_test_fed_unsold` | BASE TABLE |  |
| `ab_test_midvolga_unsold` | BASE TABLE |  |
| `arrival_on_rrc` | BASE TABLE |  |
| `audit_cash_balance` | BASE TABLE | Остатки денежных средств (ДС) на конец дня на филиале(СЕЙФ/ВСЕГО)
Используется в дашборде "Остатки ДС в кассе на конец дня" (https://metabase-sv.dns-shop.ru/dashboard/500)
Обновление раз в сутки дагом https://airflow-mv-v2.dwh.dns-shop.ru/dags/audit_cash_balance |
| `avg_potential` | MATERIALIZED VIEW |  |
| `b_big_sale` | VIEW |  |
| `b_doc` | VIEW |  |
| `b_kat_v` | VIEW |  |
| `b_op` | VIEW |  |
| `b_sale_del_06` | BASE TABLE |  |
| `b_sotr` | VIEW | Справочник сотрудников |
| `b_ter` | VIEW |  |
| `branch_attributes_history` | BASE TABLE | История изменений атрибутов филиалов |
| `branch_classification` | MATERIALIZED VIEW |  |
| `branch_claster` | BASE TABLE |  |
| `branch_configuration_model` | VIEW | Список конфигурации филиалов
(Районник, концентратор ) |
| `branch_quant` | BASE TABLE | История филиала с 2022-01-01 по текущую дату. |
| `branch_square_history` | BASE TABLE |  |
| `branch_type` | BASE TABLE | типы подразделения для дашборда "месячные показатели" |
| `buh_availab_of_doc` | BASE TABLE | Данные для дашборда Реализация - наличие документов
https://docs.google.com/spreadsheets/d/1oaPFKuoTmbcEFX7DAfnxpALf14sRa8e1pm3h9h90jFI/edit?gid=1038839709#gid=1038839709 |
| `buh_cloud_sales_registers_errors` | BASE TABLE | Для дашборда бухгалтерии(ошибки облачных касс), данные загоняются вручную |
| `buh_collection_errors` | BASE TABLE | Сведение информации по инкасации для дашборда бухгалдтерии Ошибки инкасации |
| `buh_confirmation_of_costs` | BASE TABLE | Ошибки для дашборда "Документальное подтверждение затрат" |
| `buh_costs_and_debts` | BASE TABLE | таблица для дашборда Бухгалтерия
"Затраты долги документов"
https://metabase-sv.dns-shop.ru/dashboard/95 |
| `buh_customer_credit_debt` | BASE TABLE | Данные с 2023года для дашборда "Кредиторская задолженность перед покупателями" |
| `buh_debts_ok_errors` | BASE TABLE | Сведение информации по долгам ОK для дашборда бухгалтерии Долги ОK |
| `buh_exchange_errors` | BASE TABLE | Сведение информации по обменам для дашборда бухгалтерии Ошибки обменов |
| `buh_regist_invoices` | BASE TABLE | Реестр Счет-Фактур ПОЛНЫЙ
для даша https://metabase-sv.dns-shop.ru/dashboard/87
пока из 1С запроса вручную |
| `buh_skan_sf_and_edo` | BASE TABLE | для даша бух https://metabase-sv.dns-shop.ru/dashboard/187 |
| `buh_subreport_control` | BASE TABLE | Для дашборда "Контроль подотчета" |
| `buh_work_load` | BASE TABLE | инфа по нагрузке
данные из конфы
https://confluence.dns-shop.ru/pages/viewpage.action?pageId=163414552 |
| `calculation_format_change_history` | BASE TABLE | История изменения рассчета форматов |
| `cap_quant_lite_all_dns` | BASE TABLE | Срез состояния по категориям-филиалам (Продажи, ВЕ, Остатки, Потенциалы, Лежаки ) |
| `category_direct` | BASE TABLE | Сопоставление категорий ДНС и конкурента |
| `comm_activ` | BASE TABLE |  |
| `comm_ar_sales` | BASE TABLE | Отношение количества продаж аксессуаров к основным продуктам по филиалам и месяцам. Только див. Средняя Волга |
| `comm_assessment_shipment` | BASE TABLE |  |
| `comm_asset_penalty_calculation` | BASE TABLE |  |
| `comm_avg_stoks_history_b_c_w_m` | BASE TABLE | История средних остатков |
| `comm_avg_stoks_unsold_history_b_c_w_m` | BASE TABLE | История среднего остатка лежаков |
| `comm_branch_docs` | MATERIALIZED VIEW |  |
| `comm_branch_rating` | BASE TABLE |  |
| `comm_cap_quant_company_view` | VIEW |  |
| `comm_cat_dostupnost_assortimenta` | MATERIALIZED VIEW |  |
| `comm_city_category_with_market` | BASE TABLE |  |
| `comm_city_rating_raw` | BASE TABLE |  |
| `comm_ctm_sales` | BASE TABLE | Отношение продаж СТМ к обороту по филиалам и месяцам. Только див. Средняя Волга |
| `comm_current_branch_product_price` | VIEW |  |
| `comm_current_positional_sales` | MATERIALIZED VIEW |  |
| `comm_current_positional_sales_new` | MATERIALIZED VIEW |  |
| `comm_current_potencials` | MATERIALIZED VIEW |  |
| `comm_current_product_fixes` | MATERIALIZED VIEW |  |
| `comm_current_product_raiting` | BASE TABLE | Текущий рейтиг товаров. Только по див. Средняя волга. |
| `comm_current_product_raiting_new` | BASE TABLE |  |
| `comm_current_ve` | MATERIALIZED VIEW |  |
| `comm_daily_mart` | BASE TABLE | Продажи, остатки, заявки на товар подневно по филиалам - товарам |
| `comm_dayly_sales` | MATERIALIZED VIEW |  |
| `comm_dayly_sales_2` | MATERIALIZED VIEW |  |
| `comm_dayly_stock_mv` | MATERIALIZED VIEW |  |
| `comm_dayly_stock_on_show_mv` | MATERIALIZED VIEW |  |
| `comm_dayly_znt` | MATERIALIZED VIEW |  |
| `comm_delete_shipment` | BASE TABLE |  |
| `comm_density` | BASE TABLE |  |
| `comm_distr_quant_categories_module` | BASE TABLE |  |
| `comm_distr_quant_company_view` | VIEW |  |
| `comm_distr_quant_core` | BASE TABLE | Ядро сборки дистркванта |
| `comm_distr_quant_sales_module` | BASE TABLE |  |
| `comm_distr_quant_stock_module` | BASE TABLE |  |
| `comm_filials_area_history` | BASE TABLE |  |
| `comm_filials_clusters` | BASE TABLE |  |
| `comm_formats_metric_week` | BASE TABLE |  |
| `comm_history_assortment` | BASE TABLE |  |
| `comm_inside_sum` | BASE TABLE |  |
| `comm_inside_sum_archive` | BASE TABLE | продажи конкуренты для инсайдов старого образца (без источников), не обновляется |
| `comm_merchprojects` | BASE TABLE |  |
| `comm_midvolga_dyn_d` | BASE TABLE | Дневная динамика основных коммерческих показателей в разрезе Филиал - Товар. Дивизон Средняя Волга, 2 полных предыдущих месяца + текущий месяц |
| `comm_mkf_analyze` | VIEW |  |
| `comm_mkf_dynamics` | BASE TABLE | История расчетных МКФ до дивизиону Средняя Волга из федеральнго сервера ClickHouse (adm-fspb-bi-ch2.dns-shop.ru). Регистр - RaschetnyeModeliKonfiguratsiiFilialov |
| `comm_monthly_mart` | BASE TABLE | Продажи, остатки, заявки на товар помесячно по филиалам - товарам |
| `comm_onof_categories` | VIEW |  |
| `comm_potencials_for_sq_calc` | BASE TABLE | Потенциалы продаж для расчета площадей.ююйй |
| `comm_potentials_hist_b_c` | PARTITIONED TABLE | История потенциалов в разрезе Филиал - Категория (помесячно, понедельно). Весь DNS-ритейл, с 01.01.2023 |
| `comm_product_metrics_pbi` | MATERIALIZED VIEW |  |
| `comm_product_zapret_prodazh` | BASE TABLE | Аня заполни комменты )) |
| `comm_product_zapret_prodazh_view` | VIEW |  |
| `comm_proficit_analyzer` | MATERIALIZED VIEW |  |
| `comm_prognozy_prodazh` | BASE TABLE |  |
| `comm_retail_dyn_m` | PARTITIONED TABLE |  |
| `comm_retail_dyn_w` | PARTITIONED TABLE |  |
| `comm_retail_month_dynamic_b_c` | BASE TABLE | Месячная динамика основных коммерческих показателей в разрезе Филиал - Категория. Весь DNS ритейл, с 01-01-2024 |
| `comm_retail_week_dynamic_b_c` | BASE TABLE | Недельная динамика основных коммерческих показателей в разрезе Филиал - Категория. Весь DNS ритейл, с 01-01-2024 |
| `comm_return_shipment` | MATERIALIZED VIEW |  |
| `comm_revansh` | BASE TABLE |  |
| `comm_sales_dyn_b_c_month` | BASE TABLE | Продажи по филиалу и категории помесячно |
| `comm_sales_dyn_b_c_week` | BASE TABLE | Понедельная динамика продаж по филиалу и категории |
| `comm_sales_dyn_b_c_week_tmp` | BASE TABLE |  |
| `comm_select_moves` | MATERIALIZED VIEW |  |
| `comm_shipments_statistik` | BASE TABLE |  |
| `comm_showcase` | BASE TABLE |  |
| `comm_showcase_capacity_month` | BASE TABLE | витринные емкости  |
| `comm_showcase_capacity_week` | BASE TABLE | Витринные емкости понедельно |
| `comm_showcase_stoks_d` | BASE TABLE | История остатков на витрине с 2023 года. Разрез: день-филиал-категория. Меры: шт, ску. Вся страна |
| `comm_stocks_density` | BASE TABLE |  |
| `comm_storage_cap_current` | MATERIALIZED VIEW |  |
| `comm_storage_cap_current_new` | MATERIALIZED VIEW |  |
| `comm_thermal_paper` | BASE TABLE | Остатки и рекомендуемое количество для заказа чековой ленты. Используется в рассылке маркеров |
| `comm_ugs_sales` | BASE TABLE | Отношение продаж УГС к общему обороту по филиалам, месяцам типам УГС. Только див. Средняя Волга |
| `comm_unassigned_products` | MATERIALIZED VIEW |  |
| `comm_unsold_dyn_month_lezhaki` | BASE TABLE | История лежаков с федерального сервера Formats_bi, помесячно. Разрез месяцы, филиалы, категори. По всей стране, с 01.01.2023 |
| `comm_unsold_dyn_week_lezhaki` | BASE TABLE | История лежаков понедельно. Разрез недели, филиалы, категори. По всей стране, с 01.01.2023 |
| `comm_unsold_dyn_week_potentials` | BASE TABLE | История потенциалов из федерального сервера Fomats_bi, понедельно. Разрез недели, филиалы, категории. По всей стране, с 01.01.2023 |
| `comm_unsold_history_on_stat` | PARTITIONED TABLE | История лежаков по дивизиону |
| `comm_update_daily_mart` | VIEW |  |
| `comm_upstream_pressure_on_rrc` | BASE TABLE | История входящих транзитов на РРЦ дивизиона Средняя Волга с 01.01.2024 |
| `comm_volume_filter` | VIEW |  |
| `comm_weekly_mart` | BASE TABLE | Продажи, остатки, заявки на товар понедельно по филиалам - товарам |
| `comm_zero_crossing` | BASE TABLE |  |
| `current_stock_mvideo` | BASE TABLE | таблица с категориями и остатком конкурентов |
| `current_stock_mvideo_to_del` | BASE TABLE |  |
| `current_ve` | VIEW |  |
| `daily_sales_share` | BASE TABLE | Доли продаж по дням, факт и прогноз. Используются для расчёта актива |
| `date_birth` | MATERIALIZED VIEW |  |
| `delandsale` | MATERIALIZED VIEW | Данные для дашбордов "Доставка к продажам. Магазин" и "Доставка к продажам. Сайт". 
Логистика |
| `delandsale_2` | MATERIALIZED VIEW |  |
| `delservice` | MATERIALIZED VIEW |  |
| `dict_branch` | BASE TABLE | Справочник филиалов |
| `dict_category` | BASE TABLE | Справочник категорий |
| `dict_dim_branch` | BASE TABLE |  |
| `dict_dim_product` | BASE TABLE |  |
| `dict_gfk_category` | BASE TABLE |  |
| `dict_product` | BASE TABLE | Справочник товаров |
| `dict_product_category_hierarchy` | BASE TABLE |  |
| `dictionary_categories_mvideo` | BASE TABLE |  |
| `dictionary_categories_mvideo_to_del` | BASE TABLE |  |
| `distr_quant_all_dns` | BASE TABLE | Дистр квант оригинал |
| `distr_quant_all_dns_old` | BASE TABLE |  |
| `distribution_by_author` | BASE TABLE |  |
| `distribution_recomendation` | VIEW |  |
| `div_territory_plan_all_month` | VIEW |  |
| `dko_move_product` | BASE TABLE | Таблица для сохранения перекосов ДКО |
| `dko_struct` | BASE TABLE |  |
| `dwh_temp_data_gfk` | BASE TABLE |  |
| `dwh_test` | BASE TABLE |  |
| `dynamica_mkf` | MATERIALIZED VIEW |  |
| `email_for_event_price_tag` | BASE TABLE |  |
| `employees_position_for_bot` | MATERIALIZED VIEW |  |
| `fat_client_categories_mrc` | BASE TABLE |  |
| `fed_unsold_snapshots` | BASE TABLE | НЕ УДАЛЯТЬ!!!!!!!! |
| `for_cenniki` | MATERIALIZED VIEW |  |
| `for_sim_del_06` | BASE TABLE |  |
| `for_sim_sotr_del_06` | BASE TABLE |  |
| `formats_autodistr_log_daily` | BASE TABLE | история автораспределения товаров по филиалам из КликХауса (нет наших филиалов), необходимо подключение к другому серваку(де есть данные по нашим филиалам), обновление остановлено 25,04,25 |
| `formats_transformation_store_calculator` | BASE TABLE | Расчетные данные по витринам и площадям филиалов |
| `fpu_del_07_2025` | BASE TABLE |  |
| `gfk_by_category` | BASE TABLE |  |
| `gfk_category_rrs` | BASE TABLE |  |
| `gfk_from_excel` | BASE TABLE | GFK в разрезе город-продуктовая группа. Обновляется автоматически DAG-ом gfk_from_products_dwh_in_category_mart_sv |
| `gfk_from_excel_new_format` | BASE TABLE |  |
| `gfk_from_presentations` | BASE TABLE | Распознавания презентации GFK, вручную по мере поступления данных, примерно раз в 3 месяца. Оборот раcсчитывается как произведение доли на оценку рынка. |
| `gfk_presentation_september` | BASE TABLE |  |
| `hr_employees_count` | MATERIALIZED VIEW | Количестов сотрудников на филиалах |
| `hr_returning_employees` | MATERIALIZED VIEW | Инфа по сотрудникам с причинами и датами увольнений, которые снова вернулись в компанию |
| `hr_sport_event` | BASE TABLE |  |
| `hr_sport_event_test` | BASE TABLE |  |
| `inside_dict` | BASE TABLE | справочник сведения конкурентов и магазинов DNS |
| `kpd_motivation_monitoring_of_staff_workload` | BASE TABLE |  |
| `kpi_seller` | MATERIALIZED VIEW |  |
| `log_dvizhenie_tovara_po_skladu` | MATERIALIZED VIEW |  |
| `max_fill_quant` | MATERIALIZED VIEW |  |
| `max_fill_quant_history` | BASE TABLE | История мат.вьюхи max_fill_quant |
| `merch_project_quant` | MATERIALIZED VIEW |  |
| `midvolga_warehouse_running_stocks` | BASE TABLE | Остатки товаров по филиалам и складам (див. Средняя Волга). За последние полные 7 дней |
| `minus_stock` | BASE TABLE | Минусовые остатки. Для дашборда аудита |
| `minus_stock_history` | BASE TABLE | Минусовые остатки. Для дашборда аудита |
| `minus_stock_history_del_1125` | BASE TABLE |  |
| `mkf` | VIEW |  |
| `mkf_dinamic` | VIEW | Динамика МКФ, див СВ, подставляет последние значения МКФ передыдущего месяца - следующему. |
| `monday_stock_for_last_year_to_del` | MATERIALIZED VIEW |  |
| `nesootvetstviye_ka_rn_op` | BASE TABLE | Несоответствие контрагента в Расход. накладной (документе продажи) и в оплате продажи. Для дашборда аудита |
| `nesootvetstviye_ka_rn_op_history` | BASE TABLE | Несоответствие контрагента в Расход. накладной (документе продажи) и в оплате продажи. Для дашборда аудита |
| `otgr_priem` | BASE TABLE | Данные для дашборда "Площадь филиалов" |
| `outsourcer_sv` | MATERIALIZED VIEW |  |
| `payment` | MATERIALIZED VIEW |  |
| `perekosy3_0` | MATERIALIZED VIEW |  |
| `potencial_dec` | BASE TABLE |  |
| `price_for_events` | BASE TABLE | Таблица ценников для событий (Чёрная Пятница, Новый Год), которые идут на печать |
| `price_for_events_log_from_metabase` | BASE TABLE |  |
| `price_for_events_snapshot` | BASE TABLE |  |
| `price_for_events_tmp` | BASE TABLE | Таблица для DAG price_for_events_update |
| `price_tag_current` | BASE TABLE |  |
| `price_tag_current_old` | BASE TABLE | Таблица для ценников с дефектом |
| `price_tag_current_snapshot` | BASE TABLE |  |
| `price_tag_custom_user_list` | BASE TABLE |  |
| `price_tag_custom_user_list_snapshot` | BASE TABLE |  |
| `price_tag_defect_sales_analytics` | MATERIALIZED VIEW |  |
| `price_tag_event_current_state` | MATERIALIZED VIEW | Для event ценников |
| `price_tag_event_sales_analytics` | MATERIALIZED VIEW |  |
| `price_tag_log` | BASE TABLE | Таблица для логирования причин удаления ценников |
| `price_tag_settings` | BASE TABLE | Таблица с настройками ценников |
| `price_tag_stat` | BASE TABLE | УСТАРЕЛА НЕ ИСПОЛЬЗУЕТСЯ |
| `price_tag_unsold_category` | BASE TABLE |  |
| `price_tag_unsold_category_old` | BASE TABLE | Таблица для хрнения настроек категорий для расчета ценников на лежаки |
| `price_tag_unsold_current` | BASE TABLE |  |
| `price_tag_unsold_current_snapshots` | BASE TABLE |  |
| `price_tag_unsold_current_test` | BASE TABLE |  |
| `price_tag_unsold_sales_analytics` | MATERIALIZED VIEW |  |
| `price_tag_update_price` | VIEW |  |
| `price_tags_email` | BASE TABLE | Таблица email сотрудников для отправки ценников "Локальная скидка + Лежаки" |
| `prodazhi_fed_lezhakov` | BASE TABLE |  |
| `product_fixes_daily` | BASE TABLE | Товарные фиксации итоговые, ежедневный срез потребностей |
| `product_fixes_total` | BASE TABLE | Товарные фиксации итоговые за 3 месяца, копия из dns_formats |
| `product_stat` | VIEW |  |
| `reason_for_admission` | BASE TABLE | Причина поступления. Для форматов |
| `rekl_clothes_hist` | BASE TABLE | Остатки, расходы и приходы формы для персонала на Самара Складе. Данные помесячно за последние 2 года. Используются в дашбордах отдела рекламы по остаткам формы. Обновление через даг: https://airflow-mv-v2.dwh.dns-shop.ru/dags/rekl_clothes_hist |
| `reserves_discount` | BASE TABLE | Резервы уцененного товара. Для дашборда аудита |
| `reserves_discount_history` | BASE TABLE | Резервы уцененного товара. Для дашборда аудита. |
| `reserves_movement` | BASE TABLE | Резервы перемещение товара. Для дашборда аудита |
| `reserves_movement_history` | BASE TABLE | Резервы перемещение товара. Для дашборда аудита |
| `reserves_rn` | BASE TABLE | Резервы расходных накладных. Для дашборда аудита |
| `reserves_rn_history` | BASE TABLE | Резервы расходных накладных. Для дашборда аудита |
| `reserves_tranzit` | BASE TABLE | Резервы отгрузки на транзит. Для дашборда аудита |
| `reserves_tranzit_history` | BASE TABLE | Резервы отгрузки на транзит. Для дашборда аудита |
| `rls_access_final` | BASE TABLE |  |
| `rls_dict_access` | BASE TABLE | справочник доступов по должности |
| `rls_dict_hand` | BASE TABLE |  |
| `rls_dict_sotr` | BASE TABLE | автоматически обновляющийся справочник с доступами, должностями, филиалом |
| `rp_bank_always_yes` | BASE TABLE | очищенные данные от брокера всегда да, загрузил 17.10.2025 |
| `rp_bank_always_yes_copy` | BASE TABLE |  |
| `rp_bank_applications` | BASE TABLE | Итоговая таблица по брокерам, залил 12.12.2025 |
| `rp_bank_poscredit` | BASE TABLE | очищенные данные от брокера загрузил 15.12.25 с сохранением в названиии филиала ОФП |
| `rp_metrics_sp` | BASE TABLE | Данные для Мониторинга работы с Системой поручений с 01.01.2024. ТОЛЬКО ДИВ.СВ |
| `rp_metrics_sp_div` | BASE TABLE | Данные для Мониторинга работы с Системой поручений с 01.01.2024. ОБЩИЕ даные по всем ДИВИЗИОНАМ. |
| `rp_postamate_cells_fin` | BASE TABLE | Сгруппированные данные по ячейкам постаматов по Всей сети |
| `rp_postamate_cells_raw_data` | BASE TABLE | Сырые данные из сервиса ячеек постамата, все филиалы сети, загрузка три раза в день |
| `rp_postamate_orders` | BASE TABLE | Поручения РП, история с 2025 года по всей сети |
| `rp_postamate_prod_category` | BASE TABLE | Таблица с категориями товаров. Поручения "Набор товара в постамат" по всей сети с начала 2025 |
| `rp_postomate_deadcell_hist` | BASE TABLE | История по сломанным ячейкам постоматов див СВ |
| `rp_sales` | BASE TABLE | Список продаж для создания витрин. Все Дивизионы |
| `rp_sales_0` | PARTITIONED TABLE | Список продаж для создания витрин. Все Дивизионы |
| `rp_sales_2` | BASE TABLE | Список продаж для создания витрин. Все Дивизионы |
| `rp_sales_log` | BASE TABLE |  |
| `rp_staff` | BASE TABLE | Сотрудники див СВ |
| `rp_tso_metrics_0_full` | BASE TABLE | СБОРКА. Метрики для терминалов самообслуживания
все Див/СВ до филиала + сотрудники СВ, глубина с 02.01.2023 года, месячная/недельная динамика |
| `rp_tso_metrics_2_div` | BASE TABLE | Метрики для терминалов самообслуживания
все Див, глубина с 02.01.2023 года, месячная динамика |
| `rp_tso_metrics_2_div_view_banned` | VIEW |  |
| `rp_tso_metrics_2_month` | BASE TABLE | Метрики для терминалов самообслуживания
Див СВ, глубина с 02.01.2023 года, месячная динамика |
| `rp_tso_metrics_2_week` | BASE TABLE | Метрики для терминалов самообслуживания
Див СВ, глубина с 02.01.2023 года, недельная динамика |
| `rp_tso_metrics_div` | BASE TABLE | Метрики для терминалов самообслуживания
все Дивизионы, глубина с 01.01.2023 года, месячная динамика |
| `rp_tso_metrics_month` | BASE TABLE | Метрики для терминалов самообслуживания
Див СВ, глубина с 02.01.2023 года, месячная
динамика |
| `rp_tso_metrics_week` | BASE TABLE | Метрики для терминалов самообслуживания
Див СВ, глубина с 02.01.2023 года, недельная динамика |
| `rp_tso_metrics_week_sotr` | BASE TABLE | Метрики для терминалов самообслуживания
Див СВ, глубина с 02.01.2023 года, недельная динамика |
| `rp_weekpricehistory` | BASE TABLE |  |
| `rp_weekpricehistory_product` | BASE TABLE |  |
| `rrp_from_bot_to_formats` | BASE TABLE | Для загрузки эксель файлов через бот (РРП) |
| `rs_LokalnyeLezhakiDljaRasprodazhi_snapshot` | BASE TABLE |  |
| `rs_lokalnyelezhakidljarasprodazhi_snapshot` | BASE TABLE |  |
| `rs_tseny_setkavozmozhnyhznachenij` | BASE TABLE |  |
| `sale_sotr` | BASE TABLE |  |
| `sales_promosotrudnika` | BASE TABLE | Для дашборда по промоутерам |
| `sales_turnover` | BASE TABLE |  |
| `sc_defect_partdocs` | VIEW |  |
| `sc_employee` | BASE TABLE |  |
| `sc_izd` | VIEW |  |
| `sc_mat_adretail` | MATERIALIZED VIEW |  |
| `sc_mat_ascdays` | MATERIALIZED VIEW |  |
| `sc_mat_beforenafterasc` | MATERIALIZED VIEW |  |
| `sc_mat_defect` | MATERIALIZED VIEW |  |
| `sc_mat_dno` | MATERIALIZED VIEW |  |
| `sc_mat_engdiagquality` | MATERIALIZED VIEW |  |
| `sc_mat_engfpzstatuszak` | MATERIALIZED VIEW |  |
| `sc_mat_enggivavr` | MATERIALIZED VIEW |  |
| `sc_mat_engosntfpz` | MATERIALIZED VIEW |  |
| `sc_mat_engprodrate` | MATERIALIZED VIEW |  |
| `sc_mat_engrepeat` | MATERIALIZED VIEW |  |
| `sc_mat_engworkload` | MATERIALIZED VIEW |  |
| `sc_mat_engzipmargin` | MATERIALIZED VIEW |  |
| `sc_mat_gm` | MATERIALIZED VIEW |  |
| `sc_mat_inoutall` | MATERIALIZED VIEW |  |
| `sc_mat_osnt` | MATERIALIZED VIEW |  |
| `sc_mat_paidall` | MATERIALIZED VIEW |  |
| `sc_mat_pnt` | MATERIALIZED VIEW |  |
| `sc_mat_wl_coef_logist` | MATERIALIZED VIEW |  |
| `sc_product_group` | BASE TABLE |  |
| `sc_replenishment_marker` | VIEW |  |
| `sc_replenishment_marker_hist` | BASE TABLE | Незакрытый документ Доукомплектации
Для рассылки маркеров |
| `sc_upload_wl_coef` | BASE TABLE |  |
| `sc_wl_avr` | VIEW |  |
| `sc_wl_coef_eng_docs` | MATERIALIZED VIEW |  |
| `sc_wl_coef_eng_month` | MATERIALIZED VIEW |  |
| `sc_wl_coef_eng_qt` | MATERIALIZED VIEW |  |
| `sc_wl_coef_logist` | MATERIALIZED VIEW |  |
| `sc_wl_coef_mb` | MATERIALIZED VIEW |  |
| `sc_wl_pnt` | VIEW |  |
| `schet-faktury_kolichestva` | VIEW |  |
| `sell_day` | BASE TABLE | Продажи по дням (за вчера) |
| `share_online_orders_on_tso_view` | VIEW | МЕТРИКА Доля выдач интернет-заказов на ТСО + Кол-во выдач интернет-заказов на ТСО (див. Средняя волга, с 02.01.2023 по текущую дату, группировка по филиалам, понедельно) |
| `share_payment_on_tso_view` | VIEW | МЕТРИКА Доля оплат на ТСО + Кол-во оплат на ТСО (див. Средняя волга, с 02.01.2023 по текущую дату, группировка по филиалам, понедельно) |
| `share_purchase_on_tso_view` | VIEW | МЕТРИКА Доля покупок на ТСО + Кол-во покупок на ТСО (див. Средняя волга, с 02.01.2023 по текущую дату, группировка по филиалам, понедельно) |
| `share_supermarket_on_tso_view` | VIEW | МЕТРИКА доля/количество покупок супермаркета через терминал ТСО + доля/количество количества РН,КЗ с товаром вида ценника термо в единичном экземпляре созданные в МП к общему количеству РН,КЗ на филиале. (див. Средняя волга, с 02.01.2023 по текущую дату, группировка по филиалам, понедельно) |
| `stm_za_stock_sale_del` | BASE TABLE |  |
| `stock_day2` | BASE TABLE |  |
| `stock_display` | MATERIALIZED VIEW |  |
| `stock_hist` | BASE TABLE | История изменения остатков на филиалах (филиал-товар) период - помесячно |
| `stock_hist_agr` | BASE TABLE | История изменения остатков на филиалах (филиал-категория товара) период - помесячно |
| `stock_sku_mvid_dns` | MATERIALIZED VIEW |  |
| `storehouses_quant` | MATERIALIZED VIEW |  |
| `sv_active_account_stock_b_daily` | BASE TABLE | Подневные суммарные остатки по всем счетам по филиалам |
| `sv_active_stock_b_daily` | BASE TABLE | Подневные остатки для расчета актива |
| `sv_category_hie` | VIEW |  |
| `sv_matrix_analyzer` | BASE TABLE | Витрина для оценки наполненности ширины матрицы |
| `sv_matrix_analyzer_branch` | MATERIALIZED VIEW |  |
| `sv_pfs` | MATERIALIZED VIEW |  |
| `sv_revansh_comp` | BASE TABLE |  |
| `sv_znts` | MATERIALIZED VIEW |  |
| `test_dict_dim_product` | BASE TABLE |  |
| `test_lost_sale` | VIEW |  |
| `test_poten_for_now` | BASE TABLE |  |
| `test_work_days` | BASE TABLE |  |
| `timedellog` | MATERIALIZED VIEW | Данные для дашборда "Своевременность доставки СВ". 
Логистика |
| `tmp_max_fill_for_square` | BASE TABLE |  |
| `tmp_rn_deleted` | BASE TABLE |  |
| `turnrsilog` | MATERIALIZED VIEW | Данные для дашборда "Логистические затраты и эффективность". Логистика |
| `uc_dinamic_stock` | BASE TABLE |  |
| `uc_expense_del_12_2025` | BASE TABLE |  |
| `uc_gen_del_12_2025` | BASE TABLE |  |
| `uc_kom` | BASE TABLE |  |
| `uc_oto` | BASE TABLE |  |
| `uc_prichina_ucenki` | BASE TABLE |  |
| `uc_stock_del_12_2025` | BASE TABLE |  |
| `uc_vid_ucenki` | BASE TABLE |  |
| `unclosed_transits` | BASE TABLE | Незакрытые транзиты. Данные: из GP. В выгрузку попадают документы не закрытые в срок 3 дней с момента создания документа Отгрузки на транзит, расчет производится от даты обновления выгрузки. Для дашборда аудита |
| `unclosed_transits_history` | BASE TABLE | Незакрытые транзиты. ИСТОРИЯ. Данные: из GP. В выгрузку попадают документы не закрытые в срок 14 дней с момента создания документа Отгрузки на транзит, расчет производится от даты обновления выгрузки. Для дашборда аудита |
| `unsold_midvolga_classification_snapshots` | PARTITIONED TABLE |  |
| `unsold_status_history_del_06` | BASE TABLE |  |
| `ur_case_acts_cut` | BASE TABLE |  |
| `ur_case_events` | BASE TABLE |  |
| `ur_case_il` | BASE TABLE |  |
| `ur_case_info` | BASE TABLE |  |
| `ur_case_list` | BASE TABLE |  |
| `ur_case_sides` | BASE TABLE |  |
| `ur_claim` | VIEW |  |
| `ur_court_calendar` | BASE TABLE |  |
| `ur_court_calendar_new` | BASE TABLE |  |
| `ur_court_coord` | BASE TABLE |  |
| `ur_court_info` | BASE TABLE |  |
| `ur_court_lastevent` | BASE TABLE |  |
| `ur_court_writ_of_execution` | BASE TABLE |  |
| `ur_decisions` | VIEW |  |
| `ur_mat_claim` | MATERIALIZED VIEW |  |
| `ur_mat_decisions` | MATERIALIZED VIEW |  |
| `ve_criterions` | VIEW |  |
| `ve_dynamic_month` | VIEW |  |
| `view_connections` | BASE TABLE |  |
| `viruchka` | BASE TABLE |  |
| `wa_category_volume` | VIEW |  |
| `wa_stock_sum` | VIEW |  |
| `zatr` | BASE TABLE |  |


*Сгенерировано автоматически*