<!DOCTYPE html>
<html lang="ru">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Первая мировая война 1914-1918</title>
        <style>
            * {
                margin: 0;
                padding: 0;
                box-sizing: border-box;
                font-family: 'Segoe UI', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            }
            body {
                background-color: #f5f5f5;
                color: #333;
                line-height: 1.6;
            }
            .container {
                max-width: 1200px;
                margin: 0 auto;
                padding: 0 20px;
            }
            header  {
                background: linear-gradient(rbga(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7));
                background-color: #2c3e50;
                background-size: cover;
                background-position: center;
                color: white;
                padding: 100px 0;
                text-align: center;
                margin-bottom: 40px;
            }
            header h1 {
                font-size: 3.5rem;
                margin-bottom: 20px;
                text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            }
            header p {
                font-size: 1.2rem;
                max-width: 800px;
                margin: 0 auto;
            }
            .intro {
                background-color: white;
                padding: 40px;
                border-radius: 10px;
                box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
                margin-bottom: 40px;
            }
            intro h2 {
                color: #8B0000;
                margin-bottom: 20px;
                font-size: 2rem;
            }
            intro p {
                margin-bottom: 20px;
                font-size: 1.1rem;
            }
            .years-navigation {
                display: flex;
                justify-content: center;
                flex-wrap: wrap;
                gap: 20px;
                margin: 40px 0;
            }
            .year-btn {
                background-color: #8b0000;
                color: white;
                border: none;
                padding: 15px 30px;
                font-size: 1.2rem;
                border-radius: 5px;
                cursor: pointer;
                transition: all 0.3s ease;
                text-decoration: none;
            }
            .year-btn:hover {
                background-color: #a52a2a;
                transform: translateY(-3px);
                box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            }
            .timeline {
                background-color: white;
                padding: 40px;
                border-radius: 10px;
                box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
                margin-bottom:  40px;
            }
            .timeline h2 {
                color: #8b0000;
                margin-bottom: 30px;
                font-size: 2rem;
                text-align: center;
            }
            .timeline-item {
                margin-bottom: 30px;
                padding-left: 30px;
                border-left: 3px solid#8b0000;
                position: relative;
            }
            .timeline-item:before {
                content: '';
                position: absolute;
                left: -10px;
                top: 0;
                width: 20px;
                height: 20px;
                border-radius: 50%;
                background-color: #8b0000;
            }
            .timeline-year {
                font-weight: bold;
                font-size: 1.3rem;
                color: #8b0000;
                margin-bottom: 10px;
            }
            footer {
                background-color: #333;
                color: white;
                text-align: center;
                padding: 20px 0;
                margin-top: 40px;
            }
            .year-page {
                display: none;
                padding: 40px 0;
            }
            .year-page.active {
                display: block;
            }
            .back-btn {
                background-color: #333;
                color: white;
                border: none;
                padding: 10px 20px;
                font-size: 1rem;
                border-radius: 5px;
                cursor: pointer;
                margin-bottom: 20px;
            }
            .back-btn:hover {
                background-color: #555;
            }
            .year-content {
                background-color: white;
                padding: 40px;
                border-radius: 10px;
                box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            }
            .year-content h2 {
                color: #8b0000;
                margin-bottom: 20px;
                font-size: 2.5rem;
                text-align: center;
            }
            .year-content h3 {
                color: #333;
                margin: 25px 0 15px;
                font-size: 1.5rem;
                border-bottom: 2px solid #8b0000;
                padding-bottom: 5px;
            }
            .year-content p {
                margin-bottom: 15px;
                font-size: 1.1rem;
            }
            @media (max-width: 768px) {
                header h1 {
                    font-size: 2.5rem;
                }
                .years-navigation {
                    flex-direction: column;
                    align-items: center;
                }
                .year-btn {
                    width: 80%;
                }
            }
        </style>
    </head>
    <body>
        <div id="main-page">
            <header>
                <div class="container">
                    <h1>Первая мировая война</h1>
                    <p>1914-1918: Великая война, изменившая мир</p>
                </div>
            </header>

            <div class="container">
                <section class="intro">
                    <h2>О Первой мировой войне</h2>
                    <p>Первая мировая война (28 июля 1914 года - 11 ноября 1918 года) - один из самых широкомасштабных вооружённых конфликтов в истории человечества. Война стала результатом обострения противоречий между ведущими державами мира в начале 20 века.</p>
                    <p>В войне учавствовали два противоборствующих блока: Антанта(Россия, Франция, Великобритания) и Тройственный союз(Германия, Австро-Венгрия, Болгария, Османская Империя). Впоследствии к Антанте присоединились США, Италия и другие страны.</p>
                    <p>Война привела к крушению четырёх империй: Российской, Германской, Австро-Венгерской и Османской. Общие потери составили более 20 миллионовчеловек, из которых около 10 миллионов - военные.</p>
                </section>

                <div class="years-navigation">
                    <button class="year-btn" data-year="1914">1914 год</button>
                    <button class="year-btn" data-year="1915">1915 год</button>
                    <button class="year-btn" data-year="1916">1916 год</button>
                    <button class="year-btn" data-year="1917">1917 год</button>
                    <button class="year-btn" data-year="1918">1918 год</button>
                </div>

                <section class="timeline">
                    <h2>Хронология войны</h2>
                    <div class="timeline-item">
                        <div class="timeline-year">1914 год</div>
                        <p>Начало войны, Битва на Марне, Галицийская битва</p>
                    </div>
                    <div class="timeline-item">
                        <div class="timeline-year">1915 год</div>
                        <p>Газовая атака под Ипром, Горлицкий прорыв, вступление Италии в войну</p>
                    </div>
                    <div class="timeline-item">
                        <div class="timeline-year">1916 год</div>
                        <p>Верденская мясорубка, Брусиловский прорыв, Ютландское сражение</p>
                    </div>
                    <div class="timeline-item">
                        <div class="timeline-year">1917 год</div>
                        <p>Вступления США в войну, Февральская и Октябрьская революции в России</p>
                    </div>
                    <div class="timeline-item">
                        <div class="timeline-year">1918 год</div>
                        <p>Брестский мир, Весеннее наступление, Стодневное наступление, Компьенское перемирие</p>
                    </div>
                </section>
            </div>

            <footer>
                <div class="container">
                    <p>2025 Сайт о Первой мировой войне.</p>
                </div>
            </footer>
        </div>

        <div id="1914-page" class="year-page">
            <div class="container">
                <button class="back-btn"> Назад на главную</button>
                <div class="year-content">
                    <h2>1914 год</h2>
                    <h3>Начало войны</h3>
                    <p>28 июня 1914 года в Сараево был убит эрцгерцог Франц Фердинанд, наследник Австро-Венгерского престола. Это событие стало поводом для начала войны.</p>
                    <p>28 июля Австро-Венгрия объявила войну Сербии. В течение недели в конфликт были втянуты основные европейские державы.</p>

                    <h3>Основные события</h3>
                    <p><strong>Битва на Марне</strong> (5 - 12 сентября) - стратегическая победа франко-британских войск, остановившая немецкое наступление на Париж.</p>
                    <p><strong>Галицийская битва</strong> (август - сентябрь) - крупное сражение русскими и автро-венгерскими войсками, закончившееся победой России.</p>
                    <p><strong>Первая битва при Ипре</strong> (октябрь - ноябрь) - завершение "Бега к морю" и установление Западного фронта.</p>

                    <h3>Итоги года</h3>
                    <p>К концу 1914 года война приобрела позиционный характер, особенно на Западном фронте. Планы сторон на быструю победу провалились.</p>
                </div>
            </div>
        </div>

        <div id="1915-page" class="year-page">
            <div class="container">
                <button class="back-btn"> Назад на главную</button>
                <div class="year-content">
                    <h2>1915 год</h2>
                    <h3>Расширение войны</h3>
                    <p>В 1915 году война продолжала расширяться. Италия вступила в войну на стороне Антанты, а Болгария присоединилась к Тройственному союзу.</p>

                    <h3>Основные события</h3>
                    <p><strong>Газовая атака под Ипром</strong> (22 апреля) - первое массовое применение химического оружия (хлора) нмецкими войсками.</p>
                    <p><strong>Горлицкий прорыв</strong> (май) - успешное наступление германо-австрийских войск, приведшее к "Великому отступлению" русской армии.</p>
                    <p><strong>Дарданельская операция</strong> (февраль 1915 - январь 1916) - неудачная попытка Антанты захватить проливы и вывести Османскую Империю из войны.</p>

                    <h3>Итоги года</h3>
                    <p>1915 год стал годом успехов Тройственного союза, особенно на Восточном фронте. Россия понесла тяжелые потери и утратила значительные территории.</p>
                </div>
            </div>
        </div>

        <div id="1916-page" class="year-page">
            <div class="container">
                <button class="back-btn"> Назад на главную</button>
                <div class="year-content">
                    <h2>1916 год</h2>
                    <h3>Год великих битв</h3>
                    <p>1916 год ознаменовался самыми кровопролитными сражениями войны, которые привели к огромным потерям с обеих сторон.</p>

                    <h3>Основные события</h3>
                    <p><strong>Верденская битва</strong> (февраль - декабрь) - одно из самых длительных и кровопролитных сражений в истории, получившее название "Верденская мясорубка".</p>
                    <p><strong>Битва на Сомме</strong> (июль - ноябрь) - крупнейшая битва Первой мировой войны, в которой впервые были применены танки.</p>
                    <p><strong>Брусиловский прорыв</strong> (июнь - сентябрь) - успешное наступление русских войск под командованием генерала Брусилова.</p>
                    <p><strong>Ютландское сражение</strong> (31 мая - 1 июня) - крупнейшее морское сражение войны между британским и немецким флотом.</p>

                    <h3>Итоги года</h3>
                    <p>Несмотря на огромные потери, ни одной из сторон не удалось достичь решающего перелома в войне. Стратегическая инициатива постепенно переходила к Антанте.</p>
                </div>
            </div>
        </div>

        <div id="1917-page" class="year-page">
            <div class="container">
                <button class="back-btn"> Назад на главную</button>
                <div class="year-content">
                    <h2>1917 год</h2>
                    <h3>Переломный год</h3>
                    <p>1917 год стал переломным в ходе войны. В неё вступили США, а Россия вышла из конфликта после революций.</p>

                    <h3>Основные события</h3>
                    <p><strong>Вступление США в войну</strong> (6 апреля) - после неограниченной подводной войны Германии, США объявили ей войну.</p>
                    <p><strong>Февральская революция</strong> (февраль - март) - свержение монархии в России и образование Временного правительства.</p>
                    <p><strong>Октябрьская революция</strong> (октябрь - ноябрь) - приход к власти большевиков во главе с Лениным.</p>
                    <p><strong>Битва при Капоретто</strong> (октябрь - ноябрь) - сокрушительное поражение итальяской армии от австро-венгерских и немецких войск.</p>

                    <h3>Итоги года</h3>
                    <p>Выход России из войны позволил Германии перебросить силы на Западный фронт, но вступление в войну США окончательно склонило чашу весов в пользу Антанты.</p>
                </div>
            </div>
        </div>

        <div id="1918-page" class="year-page">
            <div class="container">
                <button class="back-btn"> Назад на главную</button>
                <div class="year-content">
                    <h2>1918 год</h2>
                    <h3>Завершение войны</h3>
                    <p>1918 год стал последним годом войны. Решающие сражения привели к поражению Тройственного союза.</p>

                    <h3>Основные события</h3>
                    <p><strong>Брестский мир</strong> (3 марта) - сепаратный мирный договор между Советской Россией и Тройственным союзом.</p>
                    <p><strong>Весеннее наступление</strong> (март - июль) - последняя крупная попытка Германии добиться победы на Западном фронте.</p>
                    <p><strong>Стодневное наступление</strong> (август - ноябрь) - решающее наступление войск Антанты, приведшее к прорыву линии Гинденбурга.</p>
                    <p><strong>Компьенское перемирие</strong> (11 ноября) - подписание перемирия между Антантой и Германией, звершившее боевые действия.</p>

                    <h3>Итоги года</h3>
                    <p>Первая мировая война завершилась поражением Германии и её союзников. Война привела к координальному изменению политической карты мира и заложила предпосылки для Второй мировой войны.</p>
                </div>
            </div>
        </div>

        <script>
            document.addEventListener('DOMContentLoaded', function() {
                const yearButtons = document.querySelectorAll('.year-btn');
                const mainPage = document.getElementById('main-page');
                const yearPages = document.querySelectorAll('.year-page');
                const backButtons = document.querySelectorAll('.back-btn');

                yearButtons.forEach(button => {
                    button.addEventListener('click', function(e) {
                        e.preventDefault();
                        const year = this.getAttribute('data-year');

                        mainPage.style.display = 'none';
                        yearPages.forEach(page => {
                            page.classList.remove('active');
                            if (page.id == `${year}-page`) {
                                page.classList.add('active');
                            }
                        });
                    });
                });

                backButtons.forEach(button => {
                    button.addEventListener('click', function(e) {
                        e.preventDefault();

                        yearPages.forEach(page => {
                            page.classList.remove('active');
                        });
                        mainPage.style.display = 'block';
                    });
                });
            });
        </script>
    </body>
</html>
