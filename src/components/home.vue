<template>
    <div>
        <!-- 头部组件 -->
        <home-header></home-header>
        <!-- tabbar -->
        <div class="nav">
            <div class="navBox">
                <ul>
                    <li :class="{hov:k==0?true:false}" v-for="(item,k) in navs" :key="k">{{item}}</li>
                </ul>
            </div>
        </div>               
        <!-- 轮播 -->
        <home-swiper></home-swiper>
        <!-- 推荐 -->
        <div class="recommend">
            <h1 class="reTitle">歌单推荐</h1>
            <ul class="secondNav"> 
                <li>为你推荐</li>
                <li>90年代</li>
                <li>民谣</li>
                <li>日韩</li>
                <li>情歌</li>
                <li>网络歌曲</li>
            </ul>
            <ul class="cards_first">
                <li>
                    <img src="../assets/recommend/recommend1.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend2.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend3.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend4.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend5.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
            </ul>
        </div>
        <!-- 新歌 -->
        <div class="newSong">
            <div>
                <h1 class="reTitle" title="新歌首发">新歌首发</h1>
                <ul class="secondNav"> 
                    <li>内地</li>
                    <li>港台</li>
                    <li>欧美</li>
                    <li>日本</li>
                    <li>韩国</li>
                </ul>
                <div style="height:382px;overflow:hidden;">
                    <ul ref="one" class="list2 movein" v-show="flag==0">    
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫1</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <div class="imgBox">
                                <img src="../assets/newSong.jpg" alt="">
                                <i></i>
                            </div>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                    </ul>
                    <ul ref="two" class="list2" v-show="flag==1">    
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong2.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫2</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong2.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <div class="imgBox">
                                <img src="../assets/newSong2.jpg" alt="">
                                <i></i>
                            </div>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong2.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong2.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong2.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong2.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong2.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong2.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                    </ul>
                    <ul ref="three" class="list2" v-show="flag==2">    
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong3.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫3</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong3.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <div class="imgBox">
                                <img src="../assets/newSong3.jpg" alt="">
                                <i></i>
                            </div>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong3.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong3.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong3.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong3.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong3.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong3.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                    </ul>
                    <ul ref="four" class="list2" v-show="flag==3">    
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong4.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫4</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong4.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <div class="imgBox">
                                <img src="../assets/newSong4.jpg" alt="">
                                <i></i>
                            </div>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong4.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong4.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong4.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong4.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong4.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                        <li>
                            <div class="imgBox">
                                <img src="../assets/newSong4.jpg" alt="">
                                <i></i>
                            </div>
                            <div class="list2Box">
                                <p>躲猫猫</p>
                                <p>TFboys</p>
                            </div>
                            <div class="list2Box" style="position:absolute;right:0;">
                                <p>03:10</p>
                            </div>
                        </li>
                    </ul>
                </div>
                <ul class="pagination">
                    <li :class="{paginationActive:flag==0}"></li>
                    <li :class="{paginationActive:flag==1}"></li>
                    <li :class="{paginationActive:flag==2}"></li>
                    <li :class="{paginationActive:flag==3}"></li>
                </ul>
            </div>
            <ul class='navigation'> 
                <li @click="prev" class="el-icon-arrow-left"></li>
                <li @click="next" class="el-icon-arrow-right"></li>
            </ul>
        </div>
        <!-- 新碟推荐 -->
        <div class="recommend" style="background-image:linear-gradient(to bottom, #F1F1F1 0%, #FEFEFE 100%);">
            <h1 class="reTitle">歌单推荐</h1>
            <ul class="secondNav"> 
                <li>为你推荐</li>
                <li>90年代</li>
                <li>民谣</li>
                <li>日韩</li>
                <li>情歌</li>
                <li>网络歌曲</li>
            </ul>
            <ul class="cards_first" style="flex-wrap:wrap"> 
                <li>
                    <img src="../assets/recommend/recommend1.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend2.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend3.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend4.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend5.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li><li>
                    <img src="../assets/recommend/recommend1.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend2.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend3.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend4.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
                <li>
                    <img src="../assets/recommend/recommend5.jpg" alt="">
                    <div class="introduce">
                        <p>歌单介绍歌单介绍歌单介绍歌单介绍歌单介绍</p>
                        <p>播放量156.1万</p>
                    </div>
                    <i></i>
                </li>
            </ul>
        </div>
        <!-- 排行榜 -->
        <div class="sort">
            <h1 class="reTitle">排行榜</h1>
            <ul class="sortItems">
                <li>
                    <ul class="rotateY">
                        <li>
                            <p>巅峰榜</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>父亲</div>
                                    <div>于立伟</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>父亲</div>
                                    <div>于立伟</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>父亲</div>
                                    <div>于立伟</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>父亲</div>
                                    <div>于立伟</div>
                                </li>
                            </ul>
                        </li>
                        <li>
                            <p>巅峰榜</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>母亲</div>
                                    <div>于立伟</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>母亲</div>
                                    <div>于立伟</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>母亲</div>
                                    <div>于立伟</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>母亲</div>
                                    <div>于立伟</div>
                                </li>
                            </ul>
                        </li>
                    </ul>
                </li>
                <li>
                    <ul class="rotateY">
                        <li style="background-position:-224px 0">
                            <p>情歌榜</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>告白气球</div>
                                    <div>周杰伦</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>丫头</div>
                                    <div>王童语</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>飞云之下</div>
                                    <div>林俊杰、韩红</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>真英雄</div>
                                    <div>张卫健</div>
                                </li>
                            </ul>
                        </li>
                        <li style="background-position:-448px 0">
                            <p>情歌</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>告白气球</div>
                                    <div>周杰伦</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>丫头</div>
                                    <div>王童语</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>飞云之下</div>
                                    <div>林俊杰、韩红</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>真英雄</div>
                                    <div>张卫健</div>
                                </li>
                            </ul>
                        </li>
                    </ul>
                </li>
                <li>
                    <ul class="rotateY">
                        <li  style="background-position:-448px 0">
                            <p>情歌榜</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>告白气球</div>
                                    <div>周杰伦</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>丫头</div>
                                    <div>王童语</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>飞云之下</div>
                                    <div>林俊杰、韩红</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>真英雄</div>
                                    <div>张卫健</div>
                                </li>
                            </ul>
                        </li>
                        <li style="background-position:-672px 0">
                            <p>情歌</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>告白气球</div>
                                    <div>周杰伦</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>丫头</div>
                                    <div>王童语</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>飞云之下</div>
                                    <div>林俊杰、韩红</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>真英雄</div>
                                    <div>张卫健</div>
                                </li>
                            </ul>
                        </li>
                    </ul>
                </li>
                <li>
                    <ul class="rotateY">
                        <li style="background-position:-672px 0">
                            <p>情歌榜</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>告白气球</div>
                                    <div>周杰伦</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>丫头</div>
                                    <div>王童语</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>飞云之下</div>
                                    <div>林俊杰、韩红</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>真英雄</div>
                                    <div>张卫健</div>
                                </li>
                            </ul>
                        </li>
                        <li style="background-position:-896px 0">
                            <p>情歌</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>告白气球</div>
                                    <div>周杰伦</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>丫头</div>
                                    <div>王童语</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>飞云之下</div>
                                    <div>林俊杰、韩红</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>真英雄</div>
                                    <div>张卫健</div>
                                </li>
                            </ul>
                        </li>
                    </ul>
                </li>
                <li>
                    <ul class="rotateY">
                        <li style="background-position:-896px 0">
                            <p>情歌榜</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>告白气球</div>
                                    <div>周杰伦</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>丫头</div>
                                    <div>王童语</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>飞云之下</div>
                                    <div>林俊杰、韩红</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>真英雄</div>
                                    <div>张卫健</div>
                                </li>
                            </ul>
                        </li>
                        <li style="background-position:0 0">
                            <p>情歌</p>
                            <p>流行指数</p>
                            <i></i>
                            <ul>
                                <li>
                                    <i>1</i>
                                    <div>告白气球</div>
                                    <div>周杰伦</div>
                                </li>
                                <li>
                                    <i>2</i>
                                    <div>丫头</div>
                                    <div>王童语</div>
                                </li>
                                <li>
                                    <i>3</i>
                                    <div>飞云之下</div>
                                    <div>林俊杰、韩红</div>
                                </li> 
                                <li>
                                    <i>4</i>
                                    <div>真英雄</div>
                                    <div>张卫健</div>
                                </li>
                            </ul>
                        </li>
                    </ul>
                </li>
            </ul>
        </div>
        <!-- mv -->
        <div class="recommend Mcard" style="background-image:linear-gradient(to bottom, #F1F1F1 0%, #FEFEFE 100%);position:relative">
            <h1 class="reTitle" style="font-weight:300;">MV</h1>
            <ul class="secondNav"> 
                <li>推荐</li>
                <li>内地</li>
                <li>港台</li>
                <li>欧美</li>
                <li>日本</li>
                <li>韩国</li>
            </ul>
            <ul class="mvcard">
                <li>
                    <ul>
                        <li>
                            <img src="../assets/mvcard.png" alt="">
                            <div>
                                <p>烟花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                        <li class="behind">
                            <img src="../assets/mvcard2.png" alt="">
                            <div>
                                <p>菊花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                    </ul>
                    <i></i>
                </li>
                <li>
                    <ul>
                        <li>
                            <img src="../assets/mvcard.png" alt="">
                            <div>
                                <p>烟花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                        <li class="behind">
                            <img src="../assets/mvcard2.png" alt="">
                            <div>
                                <p>菊花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                    </ul>
                    <i></i>
                </li>
                <li>
                    <ul>
                        <li>
                            <img src="../assets/mvcard.png" alt="">
                            <div>
                                <p>烟花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                        <li class="behind">
                            <img src="../assets/mvcard2.png" alt="">
                            <div>
                                <p>菊花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                    </ul>
                    <i></i>
                </li>
                <li>
                    <ul>
                        <li>
                            <img src="../assets/mvcard.png" alt="">
                            <div>
                                <p>烟花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                        <li class="behind">
                            <img src="../assets/mvcard2.png" alt="">
                            <div>
                                <p>菊花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                    </ul>
                    <i></i>
                </li>
                <li>
                    <ul>
                        <li>
                            <img src="../assets/mvcard.png" alt="">
                            <div>
                                <p>烟花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                        <li class="behind">
                            <img src="../assets/mvcard2.png" alt="">
                            <div>
                                <p>菊花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                    </ul>
                    <i></i>
                </li>
                <li>
                    <ul>
                        <li>
                            <img src="../assets/mvcard.png" alt="">
                            <div>
                                <p>烟花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                        <li class="behind">
                            <img src="../assets/mvcard2.png" alt="">
                            <div>
                                <p>菊花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                    </ul>
                    <i></i>
                </li>
                <li>
                    <ul>
                        <li>
                            <img src="../assets/mvcard.png" alt="">
                            <div>
                                <p>烟花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                        <li class="behind">
                            <img src="../assets/mvcard2.png" alt="">
                            <div>
                                <p>菊花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                    </ul>
                    <i></i>
                </li>
                <li>
                    <ul>
                        <li>
                            <img src="../assets/mvcard.png" alt="">
                            <div>
                                <p>烟花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                        <li class="behind">
                            <img src="../assets/mvcard2.png" alt="">
                            <div>
                                <p>菊花 (《烟花》电影同名主题曲)</p>
                                <div>DAOKO</div>
                                <div><i class="el-icon-video-camera"></i>156.1万</div>
                            </div>
                        </li>
                        
                    </ul>
                    <i></i>
                </li>
            </ul>
            <div>
                <div class="cardPrev el-icon-arrow-left" @click="toggle"></div>
                <div class="cardNext el-icon-arrow-right" @click="toggle"></div>
            </div>
            <ul class="mvPagination">
                <li @click="tap(0)" :class="{paginationActive:!flagMv}"></li>
                <li @click="tap(1)" :class="{paginationActive:flagMv}"></li>
            </ul>
        </div>
        <!-- 脚 -->
        <home-footer></home-footer>
    </div>
</template>
<script>
import HeaderVue from "./header"
import HomeSwiper from "./swiper"
import FooterVue from "./footer"

    export default{
        data(){
            return {
                navs:["推荐","歌单","排行榜","主播电台","歌手","新品上架"],
                flag:0,
                msg:{name:213,age:[1,2,3,4],title:{a:1,b:1,c:1}},
                flagMv:false,
            }
        },
        watch:{
            flag(){
                if(this.flag==0){
                    var a = this;
                    setTimeout(() => {
                        a.$refs.one.className = "list2 movein";
                        a.$refs.two.className = "list2";
                        a.$refs.three.className = "list2";
                        a.$refs.four.className = "list2";
                    },0)
                }else if(this.flag==1){
                    var a = this;
                    setTimeout(() => {
                        a.$refs.one.className = "list2";
                        a.$refs.two.className = "list2 movein";
                        a.$refs.three.className = "list2";
                        a.$refs.four.className = "list2";
                    },0)
                }else if(this.flag==2){
                    var a = this;
                    setTimeout(() => {
                        a.$refs.one.className = "list2";
                        a.$refs.two.className = "list2";
                        a.$refs.three.className = "list2 movein";
                        a.$refs.four.className = "list2";
                    },0)
                }else if(this.flag==3){
                    var a = this;
                    setTimeout(() => {
                        a.$refs.one.className = "list2";
                        a.$refs.two.className = "list2";
                        a.$refs.three.className = "list2";
                        a.$refs.four.className = "list2 movein";
                    },0)
                }
            },
            flagMv(){
                // 判断true false
                var arr = [Math.random()*500,Math.random()*300,Math.random()*800,Math.random()*300,Math.random()*500,Math.random()*800,Math.random()*300];
                var elArr = document.querySelectorAll(".mvcard>li>ul");
                if(this.flagMv){
                    for(var i=0;i<elArr.length;i++){
                        this.ff(i,true)
                    }
                }else{
                    for(var i=0;i<elArr.length;i++){
                        this.ff(i,false)
                    }
                }

            },
        },
        methods:{
            prev(){
                this.flag--;
                if(this.flag==-1){
                    this.flag = 3;
                }
            },
            next(){
                this.flag++;
                if(this.flag==4){
                    this.flag=0
                }
            },
            toggle(){
                this.flagMv = !this.flagMv;
            },
            ff(s,m){
                var arr = [Math.random()*300,Math.random()*300,Math.random()*300,Math.random()*500,Math.random()*500,Math.random()*800,Math.random()*800];
                var elArr = document.querySelectorAll(".mvcard>li>ul");
                if(m){
                    setTimeout(function(){
                        elArr[s].style.transform = "rotateY(180deg)"
                    },arr[s])
                }else{
                    setTimeout(function(){
                        elArr[s].style.transform = "rotateY(0deg)"
                    },arr[s])
                }
            },
            tap(n){
                if(n==0){
                    for(var i=0;i<8;i++){
                        this.ff(i,false);
                        this.flagMv = false;
                    }
                }else if(n==1){
                    for(var i=0;i<8;i++){
                        this.ff(i,true);
                        this.flagMv = true;
                    }
                }
            }
        },
        components:{
            HomeHeader:HeaderVue,
            HomeSwiper,
            HomeFooter:FooterVue,
        }
    }
</script>
<style scoped>
    *{
        margin:0;
        padding:0;
        box-sizing: border-box;
    }
    html,body{
        overflow-x: hidden;
    }
    li{
        list-style: none;
    }
    a{
        text-decoration: none;
    }
    .nav{
        width:100%;
        height:34px;
        background:#c20c0c;
    }
    .navBox{
        margin: 0 auto;
        width:1200px;
        height:100%;
    }
    .nav ul{
        display:flex;
        justify-content: center;
        align-items:center;
        margin-left:-60px;
        width:100%;
        height:100%;
        font-size:12px;
        color:#fff;
        overflow:hidden;
    }
    .nav ul>li{
        margin-right:2%;
        line-height: 22px;
        padding:3px 15px;
        cursor:pointer;
        border-radius: 13px;
    }
    .nav ul>li:hover,.nav ul>li.hov{
        background:rgba(0,0,0,.2);
    }
    /* 推荐 */
    .reTitle{
        padding:50px 0 20px;
        font-size:1.7em;
        color:#232323;
        letter-spacing: 10px;
        text-align:center;
    }
    /* 导航栏 */
    .secondNav{
        margin-bottom:20px;
        display:flex;
        justify-content: center;
        align-items: center;
        font-size: 0.9em;
        color:#333;
    }
    .secondNav>li{
        width:80.39px;
        text-align: center;
        cursor: pointer;
    }
    .secondNav li:hover{
        color:#f46262;
    }
    /* 卡片样式 */
    .cards_first{
        margin:0 auto;
        width:1200px;
        display:flex;
        justify-content: space-around;
        align-items: flex-start;
    }
    .cards_first li{
        position:relative;
        margin-bottom:30px;
        box-sizing: border-box;
        overflow: hidden;
        width: 220px;
        height: 300px;
        font-size: 0.9em;
        border-radius: 15px;
        background: #fff;
        transition: transform 0.4s ease;
        cursor: pointer;
    }
    .cards_first li:hover{
        /* border: 1px solid transparent; */
        box-shadow: 0 10px 10px 0 rgba(0, 0, 0, 0.2);
        transform: translateY(-2%);
    }
    .cards_first li img{
        width:100%;
    }
    .cards_first li i{
        position: absolute;
        top:60px;
        left:60px;
        width:100px;
        height:100px;
        background:url(../assets/iconall.png) no-repeat;
        background-position:-8px -394px;
        transform: scale(0);
        transform-origin: center center;
        -webkit-transform-origin: center center;
        transition:transform 0.3s cubic-bezier(0.075, 0.82, 0.165, 1);
    }
    .introduce{
        margin-top:25px;
        transition: transform .4s;
    }
    .introduce>p:first-child{
        margin:5px 0;
        padding:0 2px;
        color:#000;
        font-size:0.9em;
        white-space: nowrap;
        overflow: hidden;
        text-overflow:ellipsis;
    }
    .introduce>p:last-child{
        padding:0 2px;
        color:#666;
        font-size:0.8em;
    }
    .cards_first li:hover .introduce{
        transform: translateY(-10px)
    }
    .cards_first li:hover i{
        transform:scale(0.8);
    }
    .newSong{
        position: relative;
        overflow: hidden;
        background-image: linear-gradient(to bottom, #F1F1F1 0%, #FEFEFE 100%);
    }
    .newSong>div{
        margin:0 auto;
        width:1200px;
    }

    /* 躲猫猫列表 */
    ul.list2{
        display:flex;
        justify-content: space-around;
        align-items: center;
        flex-wrap: wrap;
        align-content: flex-start;
        transition: transform .5s cubic-bezier(0.68, -0.55, 0.265, 1.55);
        transform: translateY(-400px);
    }
    .list2>li{
        display: flex;
        width: 30%;
        margin: 0 15px;
        padding: 15px 0;
        border-bottom: 1px solid #e7e4e4;
        position: relative;
    }
    .list2>li .imgBox{
        position:relative;
        float:left;
        width:96px;
        height:96px;
        overflow: hidden;
        cursor: pointer;
    }
    .list2>li .imgBox>i{
        position:absolute;
        top:-2px;
        left:-2px;
        display:inline-block;
        background:url(../assets/iconall.png) no-repeat;
        background-position:-8px -394px;
        width:100px;
        height:100px;
        transform-origin: center center;
        -webkit-transform-origin: center center;
        transform: scale(0);
        transition:transform 0.3s cubic-bezier(0.075, 0.82, 0.165, 1);
    }
    .list2>li .imgBox:hover>i{
        transform:scale(0.5);
    }

    .list2>li img{
        width:96px;
        height:96px;
    }
    .list2Box{
        margin: 23px 0 0 10px;
        font-size:1em;
        color:#333;
    }
    .list2Box>p{
        cursor:pointer;
        color:#333;
    }
    .list2Box>p:hover{
        color:#f46262;
    }
    /* navigation */
    .navigation>li{
        position: absolute;
        top:50%;
        width:79px;
        height:108px;
        background:rgba(0,0,0,.05);
        cursor: pointer;
        font-size:30px;
        text-align:center;
        line-height: 108px;
        transition: left 0.3s ease-in, right 0.3s ease-in;
    }
    .navigation>li:first-child{
        left:-79px;
    }
    .navigation>li:last-child{
        right:-79px;
    }
    .newSong:hover .navigation>li:first-child{
        left:0;
    }
    .newSong:hover .navigation>li:last-child{
        right:0;
    }
    /* pagination */
    .pagination{
        margin: 12px auto;
        display: flex;
        justify-content: center;
    }
    .pagination>li{
        background: rgba(0, 0, 0, 0.1);
        width: 12px;
        height: 12px;
        border-radius: 50%;
        margin-right: 20px;
        cursor: pointer;
    }
    .paginationActive{
        background: rgba(0, 0, 0, 0.3)!important;
    }
    .movein{
        transform: translateY(0px)!important;
    }
    /* 排行榜 */
    .sort{
        background-image: linear-gradient(to bottom, #F1F1F1 0%, #FEFEFE 100%);
    }
    .sort>ul{
        margin-bottom:25px;
        display:flex;
        justify-content: center;
        align-items: flex-start;
        transform-style: preserve-3d;
    }
    .sortItems>li{
        margin: 0 10px;
        display: flex;
        width:220px;
        height: 500px; 
        perspective: 500px;
        flex-grow: 0;
        flex-shrink: 0;
    }
    .rotateY{
        position: relative;
        width:100%;
        height:100%;
        /* backface-visibility: hidden; */
        transform-style: preserve-3d;
        transform-origin:center center -110px; 
        -webkit-transform-origin:center center -110px; 
        transition:transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        /* 视距 */

    }
    .rotateY>li{
        display: inline-block;
        position:absolute;
        top:0;
        left:0;
        width:100%;
        height:100%;
        background:url(../assets/sort.jpg) no-repeat;
    }
    .rotateY>li:last-child{
        transform-origin:center center -110px; 
        -webkit-transform-origin:center center -110px; 
        transform: rotateY(90deg);
        background-position:-224px 0;
    }
    .sortItems>li:hover>.rotateY{
        transform:rotateY(-90deg);
    }
    .rotateY>li>p{
        color:#fff;
        text-align: center;
    }
    .rotateY>li>p:first-child{
        font-size: 1.4em;
        font-weight: lighter;
        margin: 50px 0 5px;
        letter-spacing: 1px;
    }
    .rotateY>li>p:nth-child(2){
        font-weight: 500;
        font-size: 1.6em;
        letter-spacing: 2px;
        height: 42px;
        line-height: 42px;
    }
    .rotateY>li>i{
        display: block;
        width: 36px;
        height: 2px;
        background: #fff;
        margin: 28px auto;
    }
    .rotateY>li>ul>li{
        margin: 0 0 15px 26px;
        padding-left: 20px;
        position: relative;
        font-size: 1rem;
        color:#fff;
    }
    .rotateY>li>ul>li>i{
        position:absolute;
        top:0;
        left:0;
        color:#fff;
        font-style: normal;
    }
    .rotateY>li>ul>li>div{
        height: 26.5px;
        line-height: 26.5px;
    }
    /* mv */
    .mvcard{
        margin:0 auto;
        width:1200px;
        display:flex;
        justify-content: space-around;
        align-items: center;
        align-content: flex-start;
        flex-wrap: wrap;
    }
    .mvcard>li{
        position:relative;
        margin: 8px 10px;
        width: 23%;
        height: 240px;
        border-radius: 15px;
        overflow: hidden;
        /* perspective: 500px; */
        
    }
    .mvcard>li>ul{
        position: relative;
        width:100%;
        height:100%;
        transform-style: preserve-3d;
        transition:transform 0.3s cubic-bezier(0.075, 0.82, 0.165, 1);
    }
    .mvcard>li>i{
        position:absolute;
        top:calc(156.4px / 2 - 50px);
        left:calc(276px / 2 - 50px);
        width:100px;
        height:100px;
        background:url(../assets/iconall.png) no-repeat;
        background-position:-8px -394px;
        transform:scale(0);
        transition: transform 0.3s cubic-bezier(0.075, 0.82, 0.165, 1);
        cursor:pointer;
    }
    .mvcard>li:hover>i{
        transform:scale(0.5);
    }


    .mvcard ul>li{
        position:absolute;
        top:0;
        left:0;
        width:100%;
        height:100%;
        backface-visibility: hidden;
        -webkit-backface-visibility: hidden;
    }
    .mvcard ul>li>img{
        width:100%;
    }
    .mvcard ul>li>div{
        margin-left:10px;
        font-size:0.95rem;
        color:#333;
    }
    .mvcard ul>li>div>div{
        color:#777;
        margin:2px 0;
    }
    .mvcard ul>li>div>div>i{
        vertical-align: text-top;
        margin-right: 10px;
    }
    /* 背面卡片 */
    .behind{
        transform-origin:center center 0;
        -webkit-transform-origin: center center 0;
        transform: rotateY(180deg);
    }
    /* 前进后退按钮 */
    .cardPrev,.cardNext{
        position: absolute;
        top: 50%;
        margin-top: 10px;
        width: 79px;
        height: 108px;
        background: rgba(0,0,0,.05);
        opacity: 1;
        transition-property: opacity,transform;
        transition-duration: .5s;
        z-index: 2;
        cursor: pointer;
        line-height: 108px;
        text-align: center;
        font-size:30px;
        transition:left 0.3s ease-in, right 0.3s ease-in;
    }
    .cardPrev{
        left:-79px;
    }
    .cardNext{
        right:-79px;
    }
    .Mcard:hover .cardPrev{
        left:0px;
    }
    .Mcard:hover .cardNext{
        right: 0px;
    }
    .mvPagination{
        margin:12px auto;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .mvPagination>li{
        margin-right: 20px;
        background: rgba(0, 0, 0, 0.1);
        width: 12px;
        height: 12px;
        border-radius: 6px;
        cursor: pointer;
        z-index:10;
    }
    /* .pagination */
</style>