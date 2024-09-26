<script>
export default {
    name: 'MainLeagueTable',
    props: {

    },
    data() {
        return {

        }
    }
}
</script>

<template>
<div class="container d-flex main-container gap-5 mt-5 mb-4">
    <div class="league-table d-flex flex-column p-1">
        <div class="title d-flex justify-content-center mb-4">
            <h2><strong>League Table</strong></h2>
        </div>
        <table class="table">
            <thead>
                <tr class="h5">
                    <th class="bg-black text-white" scope="col" colspan="4">TEAM</th>
                    <th class="bg-black text-white" scope="col">W</th>
                    <th class="bg-black text-white" scope="col">D</th>
                    <th class="bg-black text-white" scope="col">L</th>
                    <th class="bg-black text-white ps-1" scope="col">PTS</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td class="number">1</td>
                    <td class="coat"><img src="../assets/league-club-1.png" alt=""></td>
                    <td class="name" colspan="2">Instanbul Sports</td>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tr>
                    <td class="number">1</td>
                    <td class="coat"><img src="../assets/league-club-1.png" alt=""></td>
                    <td class="name" colspan="2">Instanbul Sports</td>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tr>
                    <td class="number">1</td>
                    <td class="coat"><img src="../assets/league-club-1.png" alt=""></td>
                    <td class="name" colspan="2">Instanbul Sports</td>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tr>
                    <td class="number">1</td>
                    <td class="coat"><img src="../assets/league-club-1.png" alt=""></td>
                    <td class="name" colspan="2">Instanbul Sports</td>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tr>
                    <td class="number">1</td>
                    <td class="coat"><img src="../assets/league-club-1.png" alt=""></td>
                    <td class="name" colspan="2">Instanbul Sports</td>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tr>
                    <td class="number">1</td>
                    <td class="coat"><img src="../assets/league-club-1.png" alt=""></td>
                    <td class="name" colspan="2">Instanbul Sports</td>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tr>
                    <td class="number">1</td>
                    <td class="coat"><img src="../assets/league-club-1.png" alt=""></td>
                    <td class="name" colspan="2">Instanbul Sports</td>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tr>
                    <td class="number">1</td>
                    <td class="coat"><img src="../assets/league-club-1.png" alt=""></td>
                    <td class="name" colspan="2">Instanbul Sports</td>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tr>
                    <td class="number">1</td>
                    <td class="coat"><img src="../assets/league-club-1.png" alt=""></td>
                    <td class="name" colspan="2">Instanbul Sports</td>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tfoot class="text-center">
                    <tr>
                        <td class="bg-black text-white h5" colspan="8"><strong>View Full League Table</strong></td>
                    </tr>
                </tfoot>
            </tbody>
        </table>
    </div>

    <div class="fixtures-results">
        <div class="title d-flex justify-content-center mb-4">
            <h2><strong>Fixtures & Results</strong></h2>
        </div>
        <div class="matches-table d-flex flex-column">
            <div class="d-flex align-items-center justify-content-center matches gap-2">
                <img src="../assets/league-club-2.png" alt="">
                <p>Istanbul Sports</p>
                <p><strong>VS</strong></p>
                <p>United Fs Club</p>
                <img src="../assets/league-club-3.png" alt="">
            </div>

            <div class="d-flex align-items-center justify-content-center matches matches-b gap-2">
                <img src="../assets/league-club-2.png" alt="">
                <p>Istanbul Sports</p>
                <p><strong>VS</strong></p>
                <p>United Fs Club</p>
                <img src="../assets/league-club-3.png" alt="">
            </div>

            <div class="d-flex align-items-center justify-content-center matches gap-2">
                <img src="../assets/league-club-2.png" alt="">
                <p>Istanbul Sports</p>
                <p><strong>VS</strong></p>
                <p>United Fs Club</p>
                <img src="../assets/league-club-3.png" alt="">
            </div>

            <div class="d-flex align-items-center justify-content-center matches matches-b gap-2">
                <img src="../assets/league-club-2.png" alt="">
                <p>Istanbul Sports</p>
                <p><strong>VS</strong></p>
                <p>United Fs Club</p>
                <img src="../assets/league-club-3.png" alt="">
            </div>

            <div class="d-flex align-items-center justify-content-center matches gap-2">
                <img src="../assets/league-club-2.png" alt="">
                <p>Istanbul Sports</p>
                <p><strong>VS</strong></p>
                <p>United Fs Club</p>
                <img src="../assets/league-club-3.png" alt="">
            </div>

            <div class="d-flex align-items-center justify-content-center matches matches-b gap-2">
                <img src="../assets/league-club-2.png" alt="">
                <p>Istanbul Sports</p>
                <p><strong>VS</strong></p>
                <p>United Fs Club</p>
                <img src="../assets/league-club-3.png" alt="">
            </div>

            <div class="d-flex align-items-center justify-content-center matches gap-2">
                <img src="../assets/league-club-2.png" alt="">
                <p>Istanbul Sports</p>
                <p><strong>VS</strong></p>
                <p>United Fs Club</p>
                <img src="../assets/league-club-3.png" alt="">
            </div>

            <div class="d-flex align-items-center justify-content-center matches matches-b gap-2">
                <img src="../assets/league-club-2.png" alt="">
                <p>Istanbul Sports</p>
                <p><strong>VS</strong></p>
                <p>United Fs Club</p>
                <img src="../assets/league-club-3.png" alt="">
            </div>
            <div class="d-flex align-items-center justify-content-center matches gap-2">
                <img src="../assets/league-club-2.png" alt="">
                <p>Istanbul Sports</p>
                <p><strong>VS</strong></p>
                <p>United Fs Club</p>
                <img src="../assets/league-club-3.png" alt="">
            </div>

            <div class="d-flex align-items-center justify-content-center matches-black gap-2">
                <p class="h5"><strong>View Full Fixtures</strong></p>
            </div>
        </div>
    </div>
</div>
<div class="container">
    <img class="img-fluid" src="../assets/reklam.jpg" alt="">
</div>
</template>

<style lang="scss">
.main-container {
    img{
        height: 60px;
    }
    .league-table{
        flex-basis: 50%;
        table{
            background-color: rgb(243,243,243);
            border-left: 1px solid rgb(184, 182, 182);
            border-right: 1px solid rgb(184, 182, 182);
            thead{
                border-left: 1px solid;
                border-right: 1px solid;
            }
            .number {
                width: 30px;
            }
            td{
                border-bottom-width: 0px;
                vertical-align: baseline;
                width: 50px;
            }
            tfoot{
                height: 70px;
                border-left: 1px solid;
                border-right: 1px solid;
                tr{
                    td{
                        vertical-align: middle;
                    }
                }
            }
        }
    }
    .fixtures-results {
        flex-basis: 50%;
        
        .matches-table{
            .matches{
                height: 80px;
                background-color: rgb(243,243,243);
                height: 80.7px;
            }
            .matches-b {
                background-color: rgb(235,235,235);
            }
            .matches-black {
                height:70px;
                background-color: black;
                color: white;
            }
        }
    }
}
</style>