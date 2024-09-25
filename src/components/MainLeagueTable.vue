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
<div class="container d-flex main-container gap-5 mt-5">
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

    <div class="fixtures-results d-flex">
        <div class="title d-flex justify-content-center">
            <h1>Fixtures & Results</h1>
        </div>
    </div>
</div>
</template>

<style lang="scss" scoped>
.main-container {
    padding: 0;
    .league-table{
        width: 800px;
        table {
            td {
                vertical-align: baseline;
                background-color: rgb(245,245,245);
                border-bottom: none;
            }
            img{
                height: 60px;
            }
            .number{
                width: 20px;
            }
            .coat {
                width: 50px;
            }

            tfoot {
                height: 60px;
                td {
                    vertical-align: middle;
                }
            }
        }
    }
    .fixtures-results {
        width: 800px;
        background-color: green;
    }
}

.title, .main-table {
    width: 100%;
}
</style>