<template>
    <view class="page">
        <view class="uni-padding-wrap">
            <view class="page-section swiper1">
                <view class="page-section-spacing">
                    <swiper class="swiper1" vertical="true" :current="current">
                        <swiper-item>
                            <view class="swiper-item">
                                <view class="first">
                                    <view class="menu1" v-show="showLeft" @click="showMenu1">
                                        <image src="../../static/img/menu1.png"></image>
                                    </view>
                                    <view class="menu_box" v-show="showMenu">
                                        <view class="menu2" @click="showMenu2">
                                            <image src="../../static/img/menu2.png"></image>
                                        </view>
                                        <view class="top_menu">
                                            <view class="nav_box" @click="goFirst">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>主题</view>
                                                    <view>THEME</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box" @click="goSecond">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>单元</view>
                                                    <view>UNIT</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>创投</view>
                                                    <view>INDUSTRY</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>活动</view>
                                                    <view>EVENT</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>短⽚</view>
                                                    <view>FILMLET</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>荣誉</view>
                                                    <view>AWARDS</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>嘉宾</view>
                                                    <view>GUEST</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>⽇程</view>
                                                    <view>PROGRAM</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                        </view>
                                        <view class="bottom_menu">
                                            <view class="fot_title">
                                                <view class="title_box">创投 <br />报名</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">征片 <br />通道</view>
                                                <view class="title_status2">进行中</view>
                                            </view>

                                            <view class="fot_title">
                                                <view class="title_box">观众 <br />购票</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">活动 <br />预约</view>
                                                <view class="title_status2">进行中</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">嘉宾 <br />注册</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">媒体 <br />注册</view>
                                                <view class="title_status">待开启</view>
                                            </view>

                                            <view class="fot_title">
                                                <view class="title_box">征⽚ <br />通道</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">征⽚ <br />通道</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                        </view>
                                    </view>

                                    <view class="mobile_nav"></view>
                                    <view class="box_swiper">
                                        <image src="../../static/img/second.png"></image>
                                    </view>
                                    <view class="movie_title">平遥国际电影展</view>
                                    <view class="movie_title2"
                                        >PINGYAO CROUCHING TIGER HIDDEN DRAGON INTERNATIONAL FILM FESTIVAL</view
                                    >
                                    <view class="movie_address">中国 ⼭⻄ 晋中 平遥</view>
                                    <view class="top_hot_box">
                                        <view class="hot_heart">
                                            <view class="heart_img">
                                                <image src="../../static/img/hot2.png"></image>
                                            </view>
                                            <view class="hot_num">324</view>
                                        </view>
                                        <view class="hot_heart">
                                            <view class="heart_img">
                                                <image src="../../static/img/people.png"></image>
                                            </view>
                                            <view class="hot_num">512</view>
                                        </view>
                                    </view>
                                    <view class="icon_swiper" ref="tags">
                                        <image
                                            @mouseover="mouseOver1"
                                            @mouseleave="mouseLeave1"
                                            class="left_icon"
                                            @click="toLeft"
                                            src="../../static/img/left.png"></image>
                                        <image
                                            @mouseover="mouseOver2"
                                            @mouseleave="mouseLeave2"
                                            class="right_icon"
                                            @click="toRight"
                                            src="../../static/img/right.png"></image>
                                        <view class="icon_new" ref="tagsP">
                                            <!-- <view > -->
                                            <image
                                                v-for="(item, index) in iconArr"
                                                :key="index"
                                                class="icons_box1"
                                                :src="item.imgUrl"></image>
                                            <!-- </view> -->
                                            <!-- <image class="icons_box1" src="../../static/img/1.png"></image>
                                            <image class="icons_box1" src="../../static/img/2.png"></image>
                                            <image class="icons_box1" src="../../static/img/3.png"></image>
                                            <image class="icons_box1" src="../../static/img/4.png"></image>
                                            <image class="icons_box1" src="../../static/img/5.png"></image>
                                            <image class="icons_box1" src="../../static/img/5.png"></image>
                                            <image class="icons_box1" src="../../static/img/5.png"></image> -->
                                        </view>
                                    </view>
                                    <view class="movie_msg">
                                        <view class="chiness_msg"
                                            >平遥国际电影展（Pingyao Crouching Tiger Hidden Dragon International Film
                                            Festival）由导演贾樟柯发起创
                                            办，由⻢可·穆勒担任艺术总监，每年于拥有2700年历史的
                                            平遥古城举办。前两届电影展已于2017年及2018年成功举
                                            ⾏。在电影导演李安的特别授权下，电影展以“卧⻁藏⻰”为
                                            名，以展映⾮⻄⽅（中国、亚洲、东欧、拉丁美洲、⾮洲）
                                            影⽚为主，旨在增强中国电影与⾮⻄⽅、发展中国家电影从
                                            业者的联系和合作，形成⾮⻄⽅电影与⻄⽅电影的对话；并
                                            以严谨、负责的态度创建⼀种来⾃平遥国际电影展的精神，
                                            ⽴⾜于成为⼀个⼤格局、⼩身段的“精品电影展”，树⽴起⼀
                                            个专属于平遥国际电影展、影响⼒辐射全球的电影评价体系。
                                        </view>
                                        <view class="egls_msg"
                                            >nternational filmmakers. We also support young directors, in the hope of
                                            injecting new blood into Chinese cinema and promoting the growth of local
                                            art and culture.
                                        </view>
                                        <view class="more_msg" @click="showDetails"> 更多</view>
                                    </view>
                                    <view class="details_msg" v-show="showMovieDetails">
                                        <view class="detalis_colse" @click="closeDetails">×</view>
                                        <view class="details_chiness_msg">
                                            平遥国际电影展（Pingyao Crouching Tiger Hidden Dragon International Film
                                            Festival）由导演贾樟柯发 起创办，由⻢可·穆勒担任艺术总监，每年于拥有
                                            2700年历史的平遥古城举办。前两届电影展已于
                                            2017年及2018年成功举⾏。在电影导演李安的特别
                                            授权下，电影展以“卧⻁藏⻰”为名，以展映⾮⻄⽅
                                            （中国、亚洲、东欧、拉丁美洲、⾮洲）影⽚为主，
                                            旨在增强中国电影与⾮⻄⽅、发展中国家电影从业者
                                            的联系和合作，形成⾮⻄⽅电影与⻄⽅电影的对话；
                                            并以严谨、负责的态度创建⼀种来⾃平遥国际电影展
                                            的精神，⽴⾜于成为⼀个⼤格局、⼩身段的“精品电
                                            影展”，树⽴起⼀个专属于平遥国际电影展、影响⼒ 辐射全球的电影评价体系。
                                        </view>
                                        <view class="detials_egls_msg"
                                            >Pingyao Crouching Tiger Hidden Dragon International Film Festival(PYIFF)
                                            was founded by Chinese filmmaker Jia Zhang-ke and film historian Marco
                                            Müller. Held in Pingyao, a magnificent city with 2,700 years of history,
                                            PYIFF celebrates the achievements of international cinema and promotes the
                                            works of young Chinese directors.The year of 2017 and 2018 have seen two
                                            successful PYIFFs. With director Ang Lee's special authorization, PYIFF is
                                            named with a nod to his remarkable film Crouching Tiger, Hidden Dragon
                                            .PYIFF aims to become a professional showce fes.PYIFF encourages dialogue
                                            between non-Western (Chinese, Asian, Eastern European, Latin American, and
                                            African), and Western film communities. The aim is to strengthen links
                                            between Chinese cinema and the cinema of non-Western countries, developing
                                            countries, and regions less familiar to the Chinese public. We strive to
                                            foster communication and collaboration between Chinese and international
                                            filmmakers. We also support young directors, in the hope of injecting new
                                            blood into Chinese cinema and promoting the growth of local art and culture.
                                        </view>
                                        <view class="close2" @click="closeDetails">关闭</view>
                                    </view>
                                </view>
                            </view>
                        </swiper-item>
                        <swiper-item>
                            <view class="swiper-item">
                                <view class="second">
                                    <view class="menu1" v-show="showLeft2" @click="showMenu11">
                                        <image src="../../static/img/menu1.png"></image>
                                    </view>
                                    <view class="menu_box" v-show="showMenus2">
                                        <view class="menu2" @click="showMenu22">
                                            <image src="../../static/img/menu2.png"></image>
                                        </view>
                                        <view class="top_menu">
                                            <view class="nav_box" @click="goFirst">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>主题</view>
                                                    <view>THEME</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box" @click="goSecond">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>单元</view>
                                                    <view>UNIT</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>创投</view>
                                                    <view>INDUSTRY</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>活动</view>
                                                    <view>EVENT</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>短⽚</view>
                                                    <view>FILMLET</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>荣誉</view>
                                                    <view>AWARDS</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>嘉宾</view>
                                                    <view>GUEST</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>⽇程</view>
                                                    <view>PROGRAM</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                        </view>
                                        <view class="bottom_menu">
                                            <view class="fot_title">
                                                <view class="title_box">创投 <br />报名</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">征片 <br />通道</view>
                                                <view class="title_status2">进行中</view>
                                            </view>

                                            <view class="fot_title">
                                                <view class="title_box">观众 <br />购票</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">活动 <br />预约</view>
                                                <view class="title_status2">进行中</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">嘉宾 <br />注册</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">媒体 <br />注册</view>
                                                <view class="title_status">待开启</view>
                                            </view>

                                            <view class="fot_title">
                                                <view class="title_box">征⽚ <br />通道</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">征⽚ <br />通道</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                        </view>
                                    </view>
                                    <view class="second_top_box">
                                        <view>主题</view>
                                        <view>SLOGAN</view>
                                    </view>
                                    <view class="second_swiper">
                                        <el-carousel
                                            indicator-position="none"
                                            arrow="always"
                                            :initial-index="1"
                                            :interval="20000"
                                            :autoplay="false"
                                            type="card"
                                            height="100rpx"
                                            @change="changeSecondSwiper">
                                            <el-carousel-item v-for="(item, index) in secondArr" :key="index">
                                                <view class="nav_swiper" :class="{ newNav: result == index }">
                                                    <view>{{ item.year }}</view>
                                                    <view>{{ item.title }}</view>
                                                </view>
                                            </el-carousel-item>
                                        </el-carousel>
                                    </view>
                                    <view class="box_swiper2">
                                        <u-swiper
                                            :circular="true"
                                            height="160px"
                                            :list="swiper"
                                            @change="change"
                                            @click="click"></u-swiper>
                                    </view>
                                    <view class="top_hot_box">
                                        <view class="hot_heart">
                                            <view class="heart_img">
                                                <image src="../../static/img/hot2.png"></image>
                                            </view>
                                            <view class="hot_num">324</view>
                                        </view>
                                        <view class="hot_heart">
                                            <view class="heart_img">
                                                <image src="../../static/img/people.png"></image>
                                            </view>
                                            <view class="hot_num">512</view>
                                        </view>
                                    </view>
                                    <view class="second_fot_msg">
                                        <view class="fot_msg_title">电影，从来不是孤城</view>
                                        <view class="fot_jian_title">ONLY FILM...</view>
                                        <view class="fot_main">
                                            平遥国际电影展（Pingyao Crouching Tiger Hidden Dragon International Film
                                            Festival）由导演贾樟柯发起创
                                            办，由⻢可·穆勒担任艺术总监，每年于拥有2700年历史的
                                            平遥古城举办。前两届电影展已于2017年及2018年成功举
                                            ⾏。在电影导演李安的特别授权下，电影展以“卧⻁藏⻰”
                                            为名，以展映⾮⻄⽅（中国、亚洲、东欧、拉丁美洲、⾮
                                            洲）影⽚为主，旨在增强中国电影与⾮⻄⽅、发展中国家
                                            电影从业者的联系和合作，形成⾮⻄⽅电影与⻄⽅电影的
                                            对话；并以严谨、负责的态度创建⼀种来⾃平遥国际电影
                                            展的精神，⽴⾜于成为⼀个⼤格局、⼩身段的“精品电影 展” 。
                                        </view>
                                        <view class="fot_more" @click="showDetails2">更多</view>
                                    </view>
                                    <view class="details_msg" v-show="showMovieDetails2">
                                        <view class="detalis_colse" @click="closeDetails2">×</view>
                                        <view class="new_title">电影，从来不是孤城</view>
                                        <view class="new_title2">ONLY FILM...</view>
                                        <view class="details_chiness_msg">
                                            平遥国际电影展（Pingyao Crouching Tiger Hidden Dragon International Film
                                            Festival）由导演贾樟柯发 起创办，由⻢可·穆勒担任艺术总监，每年于拥有
                                            2700年历史的平遥古城举办。前两届电影展已于
                                            2017年及2018年成功举⾏。在电影导演李安的特别
                                            授权下，电影展以“卧⻁藏⻰”为名，以展映⾮⻄⽅
                                            （中国、亚洲、东欧、拉丁美洲、⾮洲）影⽚为主，
                                            旨在增强中国电影与⾮⻄⽅、发展中国家电影从业者
                                            的联系和合作，形成⾮⻄⽅电影与⻄⽅电影的对话；
                                            并以严谨、负责的态度创建⼀种来⾃平遥国际电影展
                                            的精神，⽴⾜于成为⼀个⼤格局、⼩身段的“精品电
                                            影展”，树⽴起⼀个专属于平遥国际电影展、影响⼒ 辐射全球的电影评价体系。
                                        </view>
                                        <view class="detials_egls_msg"
                                            >Pingyao Crouching Tiger Hidden Dragon International Film Festival(PYIFF)
                                            was founded by Chinese filmmaker Jia Zhang-ke and film historian Marco
                                            Müller. Held in Pingyao, a magnificent city with 2,700 years of history,
                                            PYIFF celebrates the achievements of international cinema and promotes the
                                            works of young Chinese directors.The year of 2017 and 2018 have seen two
                                            successful PYIFFs. With director Ang Lee's special authorization, PYIFF is
                                            named with a nod to his remarkable film Crouching Tiger, Hidden Dragon
                                            .PYIFF aims to become a professional showce fes.PYIFF encourages dialogue
                                            between non-Western (Chinese, Asian, Eastern European, Latin American, and
                                            African), and Western film communities. The aim is to strengthen links
                                            between Chinese cinema and the cinema of non-Western countries, developing
                                            countries, and regions less familiar to the Chinese public. We strive to
                                            foster communication and collaboration between Chinese and international
                                            filmmakers. We also support young directors, in the hope of injecting new
                                            blood into Chinese cinema and promoting the growth of local art and culture.
                                        </view>
                                        <view class="close2" @click="closeDetails2">关闭</view>
                                    </view>
                                </view>
                            </view>
                        </swiper-item>
                        <swiper-item>
                            <view class="swiper-item">
                                <view class="third">
                                    <view class="menu1" v-show="showLeft3" @click="showMenu111">
                                        <image src="../../static/img/menu1.png"></image>
                                    </view>
                                    <view class="menu_box" v-show="showMenus3">
                                        <view class="menu2" @click="showMenu222">
                                            <image src="../../static/img/menu2.png"></image>
                                        </view>
                                        <view class="top_menu">
                                            <view class="nav_box" @click="goFirst">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>主题</view>
                                                    <view>THEME</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box" @click="goSecond">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>单元</view>
                                                    <view>UNIT</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>创投</view>
                                                    <view>INDUSTRY</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>活动</view>
                                                    <view>EVENT</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>短⽚</view>
                                                    <view>FILMLET</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>荣誉</view>
                                                    <view>AWARDS</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>嘉宾</view>
                                                    <view>GUEST</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                            <view class="nav_box">
                                                <image class="nav_box_img" src="../../static/img/topNav.png"></image>
                                                <view class="nav_box_msg">
                                                    <view>⽇程</view>
                                                    <view>PROGRAM</view>
                                                </view>
                                                <image class="nav_box_img" src="../../static/img/topNav2.png"></image>
                                            </view>
                                        </view>
                                        <view class="bottom_menu">
                                            <view class="fot_title">
                                                <view class="title_box">创投 <br />报名</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">征片 <br />通道</view>
                                                <view class="title_status2">进行中</view>
                                            </view>

                                            <view class="fot_title">
                                                <view class="title_box">观众 <br />购票</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">活动 <br />预约</view>
                                                <view class="title_status2">进行中</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">嘉宾 <br />注册</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">媒体 <br />注册</view>
                                                <view class="title_status">待开启</view>
                                            </view>

                                            <view class="fot_title">
                                                <view class="title_box">征⽚ <br />通道</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                            <view class="fot_title">
                                                <view class="title_box">征⽚ <br />通道</view>
                                                <view class="title_status">待开启</view>
                                            </view>
                                        </view>
                                    </view>
                                    <view class="third_top_box">
                                        <view>单元</view>
                                        <view>SLOGAN</view>
                                    </view>
                                    <view class="second_swiper">
                                        <el-carousel
                                            indicator-position="none"
                                            arrow="always"
                                            :initial-index="1"
                                            :interval="4000"
                                            :autoplay="false"
                                            type="card"
                                            height="100rpx"
                                            @change="changeSecondSwiper2">
                                            <el-carousel-item v-for="(item, index) in thirdArr" :key="index">
                                                <view class="nav_swiper" :class="{ newNav2: result2 == index }">
                                                    <view>{{ item.title }}</view>
                                                    <view>{{ item.eGls }}</view>
                                                </view>
                                            </el-carousel-item>
                                        </el-carousel>
                                    </view>
                                    <view class="third_center_box">
                                        <view class="fang"></view>
                                        <view class="main_box_center">
                                            <span>
                                                年度重要导演的作品、备受关注的优秀影⽚的
                                                红毯⾸映年度重要导演的作品、备受关注的优
                                                秀影⽚的红毯⾸映年度重要导演的作品、备受 关注的优秀影⽚
                                            </span>
                                        </view>
                                    </view>
                                    <view class="movie_box">
                                        <view
                                            class="movie_details_box"
                                            v-for="item in 4"
                                            :key="item"
                                            @click="showMovie">
                                            <view class="movie_img_box">
                                                <image src="../../static/img/movie_details.jpg"></image>
                                            </view>
                                            <view class="movie_title">
                                                <span>电影，从来不是孤城</span>
                                            </view>
                                            <view class="movie_agls">
                                                <span>ONLY FILM…</span>
                                            </view>
                                            <view class="movie_name">
                                                <span>平遥国际电影展</span>
                                            </view>
                                        </view>
                                    </view>

                                    <view class="details_msg" v-show="showMovieDetails3">
                                        <view class="detalis_colse" @click="closeDetails3">×</view>
                                        <view class="new_title">电影，从来不是孤城</view>
                                        <view class="new_title2">ONLY FILM...</view>
                                        <view class="details_chiness_msg">
                                            平遥国际电影展（Pingyao Crouching Tiger Hidden Dragon International Film
                                            Festival）由导演贾樟柯发 起创办，由⻢可·穆勒担任艺术总监，每年于拥有
                                            2700年历史的平遥古城举办。前两届电影展已于
                                            2017年及2018年成功举⾏。在电影导演李安的特别
                                            授权下，电影展以“卧⻁藏⻰”为名，以展映⾮⻄⽅
                                            （中国、亚洲、东欧、拉丁美洲、⾮洲）影⽚为主，
                                            旨在增强中国电影与⾮⻄⽅、发展中国家电影从业者
                                            的联系和合作，形成⾮⻄⽅电影与⻄⽅电影的对话；
                                            并以严谨、负责的态度创建⼀种来⾃平遥国际电影展
                                            的精神，⽴⾜于成为⼀个⼤格局、⼩身段的“精品电
                                            影展”，树⽴起⼀个专属于平遥国际电影展、影响⼒ 辐射全球的电影评价体系。
                                        </view>
                                        <view class="detials_egls_msg"
                                            >Pingyao Crouching Tiger Hidden Dragon International Film Festival(PYIFF)
                                            was founded by Chinese filmmaker Jia Zhang-ke and film historian Marco
                                            Müller. Held in Pingyao, a magnificent city with 2,700 years of history,
                                            PYIFF celebrates the achievements of international cinema and promotes the
                                            works of young Chinese directors.The year of 2017 and 2018 have seen two
                                            successful PYIFFs. With director Ang Lee's special authorization, PYIFF is
                                            named with a nod to his remarkable film Crouching Tiger, Hidden Dragon
                                            .PYIFF aims to become a professional showce fes.PYIFF encourages dialogue
                                            between non-Western (Chinese, Asian, Eastern European, Latin American, and
                                            African), and Western film communities. The aim is to strengthen links
                                            between Chinese cinema and the cinema of non-Western countries, developing
                                            countries, and regions less familiar to the Chinese public. We strive to
                                            foster communication and collaboration between Chinese and international
                                            filmmakers. We also support young directors, in the hope of injecting new
                                            blood into Chinese cinema and promoting the growth of local art and culture.
                                        </view>
                                        <view class="close2" @click="closeDetails3">关闭</view>
                                    </view>
                                </view>
                            </view>
                        </swiper-item>
                    </swiper>
                </view>
            </view>
        </view>
    </view>
</template>

<script>
    export default {
        name: '',
        // 数据参数
        data() {
            return {
                result: 1,
                result2: 1,
                showMovieDetails: false,
                showMovieDetails2: false,
                showMovieDetails3: false,
                showMenu: false,
                showMenus2: false,
                showMenus3: false,
                showLeft: true,
                showLeft2: true,
                showLeft3: true,
                current: 0,
                leftresult: true,
                rightresult: true,
                iconArr: [
                    {
                        imgUrl: '../../static/img/1.png',
                    },
                    {
                        imgUrl: '../../static/img/2.png',
                    },
                    {
                        imgUrl: '../../static/img/3.png',
                    },
                    {
                        imgUrl: '../../static/img/4.png',
                    },
                    {
                        imgUrl: '../../static/img/4.png',
                    },
                    {
                        imgUrl: '../../static/img/5.png',
                    },
                    {
                        imgUrl: '../../static/img/1.png',
                    },
                ],
                secondArr: [
                    {
                        year: 2022,
                        title: '第七届',
                    },
                    {
                        year: 2022,
                        title: '第六届',
                    },
                    {
                        year: 2021,
                        title: '第五届',
                    },
                    {
                        year: 2020,
                        title: '第四届',
                    },
                    {
                        year: 2019,
                        title: '第三届',
                    },
                ],
                thirdArr: [
                    {
                        title: '从山西出发',
                        eGls: 'CROUCHING TIGERS',
                    },
                    {
                        title: '藏龙',
                        eGls: 'HIDDEN DRAGONS',
                    },
                    {
                        title: '回顾/致敬',
                        eGls: 'GALAS',
                    },
                ],

                swiper: [
                    {
                        url: '../../static/img/banner.jpg',
                        title: '标题1',
                    },
                    {
                        url: '../../static/img/banner2.jpg',
                        title: '标题2',
                    },
                    {
                        url: '../../static/img/banner3.jpg',
                        title: '标题3',
                    },
                ],
            };
        },
        /*
      监听页面加载函数
    */
        onLoad() {},
        /*
      监听页面显示加载函数
    */
        onShow() {
            console.log(this.iconArr);

            // var mySwiper = new Swiper('.swiper', {
            //     direction: 'horizontal', // 垂直切换选项
            //     // loop: true, // 循环模式选项
            //     slidesPerView: 3,
            //     // 如果需要分页器
            //     // pagination: {
            //     //     el: '.swiper-pagination',
            //     // },
            //     // 如果需要前进后退按钮
            //     navigation: {
            //         nextEl: '.swiper-button-next',
            //         prevEl: '.swiper-button-prev',
            //     },
            //     // 如果需要滚动条
            //     // scrollbar: {
            //     //     el: '.swiper-scrollbar',
            //     // },
            // });
        },
        /*
      事件处理函数
    */
        mounted() {
            // 获取nav_box的类名，当点击其中某一项，就把字体设置为黄色，其他的设置为白色
            var nav_box = document.getElementsByClassName('nav_box');
            for (var i = 0; i < nav_box.length; i++) {
                nav_box[i].onclick = function () {
                    for (var j = 0; j < nav_box.length; j++) {
                        nav_box[j].style.color = '#fff';
                    }
                    this.style.color = '#ddaf2d';
                };
            }
            if (document != undefined) {
                document.getElementsByClassName('uni-placeholder')[0].style.display = 'none';
                document.getElementsByClassName('uni-page-head')[0].style.display = 'none';
            }
        },
        methods: {
            // 导航控制
            goFirst() {
                this.current = 1;
                this.showMenu = false;
                this.showMenus2 = false;
                this.showMenus3 = false;
            },
            goSecond() {
                this.current = 2;
                this.showMenu = false;
                this.showMenus2 = false;
                this.showMenus3 = false;
            },
            showMovie() {
                this.showMovieDetails3 = true;
            },
            click(e) {},
            change(e) {},
            changeSecondSwiper(i) {
                console.log('i: ', i);
                this.result = i;
            },
            changeSecondSwiper2(i) {
                console.log('i: ', i);
                this.result2 = i;
            },
            // 控制菜单显示与隐藏
            showMenu1() {
                this.showMenu = true;
            },
            showMenu11() {
                this.showMenus2 = true;
            },
            showMenu111() {
                this.showMenus3 = true;
            },
            showMenu2() {
                this.showMenu = false;
            },
            showMenu22() {
                this.showMenus2 = false;
            },
            showMenu222() {
                this.showMenus3 = false;
            },
            // 电影详情
            showDetails() {
                this.showMovieDetails = true;
            },
            showDetails2() {
                this.showMovieDetails2 = true;
            },
            closeDetails() {
                this.showMovieDetails = false;
            },
            closeDetails2() {
                this.showMovieDetails2 = false;
            },
            closeDetails3() {
                this.showMovieDetails3 = false;
            },
            mouseOver1() {
                this.leftresult = false;
            },
            mouseLeave1() {
                this.leftresult = true;
            },
            mouseOver2() {
                this.rightresult = false;
            },
            mouseLeave2() {
                this.rightresult = true;
            },
            moveSlow(distance, total, step, LOR) {
                // 正向滚动 和 反向滚动
                if (LOR) {
                    // 每隔1毫秒移动一小段距离，直到移动至目标至为止，反之亦然
                    if (distance < total) {
                        distance += step;
                        this.$refs.tagsP.scrollLeft = distance;
                        setTimeout(() => {
                            this.moveSlow(distance, total, step, true);
                        }, 1);
                    } else {
                        this.$refs.tagsP.scrollLeft = total;
                    }
                } else if (!LOR) {
                    if (distance > total) {
                        distance -= step;
                        this.$refs.tagsP.scrollLeft = distance;
                        setTimeout(() => {
                            this.moveSlow(distance, total, step, false);
                        }, 1);
                    } else {
                        this.$refs.tagsP.scrollLeft = total;
                    }
                }
            },
            toRight() {
                // 获取 items 数组的第一个元素
                let first = this.iconArr[0];
                // 将第一个元素从数组中删除
                this.iconArr.splice(0, 1);
                // 将第一个元素添加到数组的末尾
                this.iconArr.push(first);
                // 往右滚动
                // this.$refs.tagsP.scrollLeft = this.scrollNum;
                let distance = this.$refs.tagsP.scrollLeft;

                let scrollNum = distance + 200;
                let step = (distance - scrollNum) / 50;
                if (step < 0) step = -step;
                this.moveSlow(distance, scrollNum, step, true);
            },
            toLeft() {
                // 获取 items 数组的最后一个元素
                let last = this.iconArr[this.iconArr.length - 1];
                // 将最后一个元素从数组中删除
                this.iconArr.splice(this.iconArr.length - 1, 1);
                // 将最后一个元素添加到数组的开头
                this.iconArr.unshift(last);
                // 左滚动
                // let distance = this.$refs.tagsP.scrollLeft;
                // let scrollNum = distance - 200;
                // if (scrollNum < 0) {
                //     scrollNum = 0;
                // }
                // let step = (distance - scrollNum) / 50;
                // if (step < 0) step = -step;
                // this.moveSlow(distance, scrollNum, step, false);
            },
        },
        /*
      监听页面初次渲染完成
    */
        onReady() {},
        /*
      监听监听页面隐藏
    */
        onHide() {},
        /*
      监听页面卸载
    */
        onUnload() {},
        /*
      监听窗口尺寸变化
    */
        onResize() {},
        /*
      监听用户下拉动作
    */
        onPullDownRefresh() {},
        /*
      页面滚动到底部的事件
    */
        onReachBottom() {},
        /*
      点击 tab 时触发
    */
        onTabItemTap() {},
        /*
      用户点击右上角分享
    */
        onShareAppMessage() {},
        /*
      监听页面滚动
    */
        onPageScroll() {},
        /*
      组件绑定
    */
        components: {},
        /*
      侦听器
    */
        watch: {},
        /*
      计算属性
    */
        computed: {},
    };
</script>

<style lang="scss" scoped>
    .newNav {
        color: #fff !important;
        font-size: 18px !important;
    }
    .newNav2 {
        color: #fff !important;
        // font-size: 18px ;
        view:nth-child(1) {
            font-size: 25px !important;
            font-weight: bold;
        }
        view:nth-child(2) {
            font-size: 11px !important;
        }
    }

    /deep/.el-carousel__mask {
        width: 100%;
        background-color: #fff0;
        opacity: 0.24;
        -webkit-transition: 0.2s;
        transition: 0.2s;
    }
    .third {
        padding: 52rpx;
        background-color: pink;
        background-image: linear-gradient(
                rgba(182, 182, 182, 0.5),
                rgba(182, 182, 182, 0.5),
                rgba(59, 59, 59, 0.5),
                rgba(9, 9, 9, 0.5),
                rgba(9, 9, 9, 0.5),
                rgba(9, 9, 9, 0.8),
                rgba(0, 0, 0, 0.9)
            ),
            url(../../static/img/index.png);
        background-size: 100% 100%;
        background-repeat: no-repeat;
        height: 100vh;
        .details_msg {
            width: 80%;
            height: 90%;
            margin: 0 auto;
            position: absolute;
            top: 3%;
            z-index: 99;
            background-color: rgba(9, 9, 9, 0.9);
            padding: 20rpx 30rpx 20rpx 30rpx;
            color: #fff;
            .new_title {
                font-size: 18px;
                text-align: center;
                margin-top: 60rpx;
            }
            .new_title2 {
                font-size: 11px;
                text-align: center;
            }
            .detalis_colse {
                color: #000;
                float: right;
                border-radius: 50%;
                width: 50rpx;
                height: 50rpx;
                font-weight: bold;
                text-align: center;
                line-height: 50rpx;
                font-size: 27px;
                background-color: #ddaf2d;
            }
            .details_chiness_msg {
                margin-top: 36rpx;
                font-size: 12px;
                margin-bottom: 20rpx;
            }
            .detials_egls_msg {
                font-size: 12px;
            }
            .close2 {
                width: 100rpx;
                padding: 10rpx;
                font-size: 12px;
                background-color: #ddaf2d;
                color: #000;
                text-align: center;
                border-radius: 100rpx;
                margin-top: 10rpx;
                margin: 0 auto;
                position: absolute;
                bottom: 5%;
                left: 50%;
                transform: translateX(-50%);
            }
        }
        .second_fot_msg {
            color: #fff;
            .fot_msg_title {
                font-size: 39rpx;
            }
            .fot_jian_title {
                font-size: 20rpx;
            }
            .fot_main {
                margin-top: 20rpx;
                font-size: 13px;
            }
            .fot_more {
                font-size: 14px;
                color: #ddaf2d;
                margin-top: 20rpx;
                text-align: right;
            }
        }
        .top_hot_box {
            display: flex;
            height: 70rpx;
            justify-content: flex-end;
            align-items: center;
            padding: 30rpx 0 30rpx 0;
            margin-top: 20rpx;
            .hot_heart {
                width: 27%;
                height: 100%;
                display: flex;
                align-items: center;
                justify-content: space-between;
                .hot_num {
                    width: 50%;
                    color: #ffffff;
                }
                .heart_img {
                    width: 40%;
                    height: 100%;
                    image {
                        width: 100%;
                        height: 100%;
                    }
                }
            }
        }
        .box_swiper2 {
            width: 100%;
            // height: 60px;
            margin: 30rpx auto;
            image {
                width: 40%;
                height: 100%;
            }
        }
        .movie_box {
            margin-top: 20rpx;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            .movie_details_box {
                width: 40%;
                margin-top: 20rpx;

                .movie_img_box {
                    width: 100%;
                    height: 280rpx;
                    image {
                        width: 100%;
                        height: 100%;
                    }
                }
                .movie_title {
                    margin-top: 10rpx;
                    font-size: 14px;
                    color: #ddaf2d;
                    text-align: center;
                    font-weight: bold;
                    span {
                        background: rgba(110, 110, 110, 0.5);
                    }
                }
                .movie_agls {
                    font-size: 11px;
                    color: #ffffff;
                    text-align: center;
                    span {
                        background: rgba(110, 110, 110, 0.5);
                    }
                }
                .movie_name {
                    font-size: 12px;
                    color: #ffffff;
                    text-align: center;
                    span {
                        background: rgba(110, 110, 110, 0.5);
                    }
                }
            }
        }
        .third_center_box {
            display: flex;
            width: 100%;
            height: 80px;
            margin-top: 20rpx;
            .fang {
                width: 330px;
                // width: 95%;
                height: 100%;
                background-color: #ffffff;
                display: block;
            }
            .main_box_center {
                color: rgb(238, 238, 238);
                margin-left: 10rpx;
                // 超出第4行隐藏显示...
                overflow: hidden;
                text-overflow: ellipsis;
                display: -webkit-box;
                -webkit-line-clamp: 4;
                -webkit-box-orient: vertical;
                height: 100%;
                // 文字背景灰色
                span {
                    background: rgba(110, 110, 110, 0.5);
                }
            }
        }
        .third_top_box {
            text-align: center;
            color: #ddaf2d;
            margin-top: -4%;
        }
        .third_top_box view:nth-child(1) {
            font-size: 54rpx;
            font-weight: bold;
            letter-spacing: 10rpx;
        }
        .third_top_box view:nth-child(2) {
            font-size: 12px;
        }
        .second_swiper {
            margin-top: 40rpx;
            width: 119%;
            margin-left: -10%;
            line-height: 52rpx;
            .nav_swiper {
                text-align: center;
                // line-height: 200rpx;
                display: flex;
                flex-direction: column;
                margin-left: 10px;
                margin-right: 10px;
                color: #bebebe;
            }
            .nav_swiper view:nth-child(11) {
                font-size: 30px;
            }
            .nav_swiper view:nth-child(2) {
                font-size: 11px;
            }
        }

        .menu_box {
            width: 60%;
            height: 100vh;
            position: absolute;
            left: 0;
            top: 0;
            z-index: 99;
            background-color: rgb(100, 100, 100);
            .menu2 {
                border-radius: 50%;
                background-color: #ddaf2d;
                width: 35px;
                height: 35px;
                position: absolute;
                top: 1%;
                right: 2%;
                text-align: center;
                image {
                    width: 70%;
                    height: 70%;
                    top: 15%;
                }
            }
            .bottom_menu {
                display: flex;
                flex-wrap: wrap;
                justify-content: space-between;
                width: 90%;
                // height: 40%;
                margin: 30rpx auto 0;
                .fot_title {
                    width: 44%;

                    height: 70px;
                    // 渐变灰色
                    background-image: linear-gradient(
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgba(182, 182, 182, 0.8),
                        rgba(182, 182, 182, 0.7),
                        rgba(182, 182, 182, 0.8),
                        rgba(59, 59, 59, 0.5)
                    );
                    border-radius: 10px;
                    position: relative;
                    margin-right: 10rpx;
                    margin-bottom: 30rpx;
                    .title_box {
                        text-align: center;
                        color: #000;
                        font-size: 15px;
                        padding: 8rpx;
                    }
                    .title_status {
                        text-align: center;
                        color: #fff;
                        font-size: 12px;
                        border-radius: 0 0 10px 10px;
                        background-color: #000;
                        height: 23px;
                        line-height: 23px;
                        position: absolute;
                        width: 100%;
                        bottom: 0;
                    }
                    .title_status2 {
                        text-align: center;
                        color: #000;
                        font-size: 12px;
                        border-radius: 0 0 10px 10px;
                        background-color: #ddaf2d;
                        height: 23px;
                        line-height: 23px;
                        position: absolute;
                        width: 100%;
                        bottom: 0;
                    }
                }
            }
            .top_menu {
                display: flex;
                flex-wrap: wrap;
                width: 90%;
                height: 40%;
                margin: 90rpx auto 0;
                // background-color: pink;
                .nav_box {
                    display: flex;
                    width: 50%;
                    height: 100rpx;
                    text-align: center;
                    line-height: 42rpx;
                    color: #ffffff;

                    .nav_box_img {
                        width: 16%;
                        height: 100%;
                    }
                    .nav_box_msg {
                        width: 60%;
                    }
                    .nav_box_msg view:nth-child(1) {
                        font-size: 13px;
                    }
                    .nav_box_msg view:nth-child(2) {
                        font-size: 13px;
                    }
                }
            }
        }
        .menu1 {
            border-radius: 50%;
            background-color: #ddaf2d;
            width: 35px;
            height: 35px;
            position: absolute;
            top: 1%;
            left: 2%;
            text-align: center;
            image {
                width: 70%;
                height: 70%;
                top: 15%;
            }
        }
    }
    .second {
        padding: 52rpx;
        background-color: pink;
        background-image: linear-gradient(
                rgba(182, 182, 182, 0.5),
                rgba(182, 182, 182, 0.5),
                rgba(59, 59, 59, 0.5),
                rgba(9, 9, 9, 0.5),
                rgba(9, 9, 9, 0.5),
                rgba(9, 9, 9, 0.8),
                rgba(0, 0, 0, 0.9)
            ),
            url(../../static/img/index.png);
        background-size: 100% 100%;
        background-repeat: no-repeat;
        height: 100vh;
        .details_msg {
            width: 80%;
            height: 90%;
            margin: 0 auto;
            position: absolute;
            top: 3%;
            z-index: 99;
            background-color: rgba(9, 9, 9, 0.9);
            padding: 20rpx 30rpx 20rpx 30rpx;
            color: #fff;
            .new_title {
                font-size: 18px;
                text-align: center;
                margin-top: 60rpx;
            }
            .new_title2 {
                font-size: 11px;
                text-align: center;
            }
            .detalis_colse {
                color: #000;
                float: right;
                border-radius: 50%;
                width: 50rpx;
                height: 50rpx;
                font-weight: bold;
                text-align: center;
                line-height: 50rpx;
                font-size: 27px;
                background-color: #ddaf2d;
            }
            .details_chiness_msg {
                margin-top: 36rpx;
                font-size: 12px;
                margin-bottom: 20rpx;
            }
            .detials_egls_msg {
                font-size: 12px;
            }
            .close2 {
                width: 100rpx;
                padding: 10rpx;
                font-size: 12px;
                background-color: #ddaf2d;
                color: #000;
                text-align: center;
                border-radius: 100rpx;
                margin-top: 10rpx;
                margin: 0 auto;
                position: absolute;
                bottom: 5%;
                left: 50%;
                transform: translateX(-50%);
            }
        }
        .second_fot_msg {
            color: #fff;
            .fot_msg_title {
                font-size: 39rpx;
            }
            .fot_jian_title {
                font-size: 20rpx;
            }
            .fot_main {
                margin-top: 20rpx;
                font-size: 13px;
            }
            .fot_more {
                font-size: 14px;
                color: #ddaf2d;
                margin-top: 20rpx;
                text-align: right;
            }
        }
        .top_hot_box {
            display: flex;
            height: 70rpx;
            justify-content: flex-end;
            align-items: center;
            padding: 30rpx 0 30rpx 0;
            margin-top: 20rpx;
            .hot_heart {
                width: 27%;
                height: 100%;
                display: flex;
                align-items: center;
                justify-content: space-between;
                .hot_num {
                    width: 50%;
                    color: #ffffff;
                }
                .heart_img {
                    width: 40%;
                    height: 100%;
                    image {
                        width: 100%;
                        height: 100%;
                    }
                }
            }
        }
        .box_swiper2 {
            width: 100%;
            // height: 60px;
            margin: 30rpx auto;
            image {
                width: 40%;
                height: 100%;
            }
        }
        .second_top_box {
            text-align: center;
            color: #ddaf2d;
            margin-top: -4%;
        }
        .second_top_box view:nth-child(1) {
            font-size: 60rpx;
            font-weight: bold;
            letter-spacing: 10rpx;
        }
        .second_top_box view:nth-child(2) {
            font-size: 15px;
        }
        .second_swiper {
            margin-top: 40rpx;
            .nav_swiper {
                text-align: center;
                // line-height: 200rpx;
                display: flex;
                flex-direction: column;
                color: #bebebe;
            }
            .nav_swiper view:nth-child(1) {
                font-size: 30px;
                font-weight: bold;
            }
            .nav_swiper view:nth-child(2) {
                font-size: 12px;
            }
        }

        .menu_box {
            width: 60%;
            height: 100vh;
            position: absolute;
            left: 0;
            top: 0;
            z-index: 99;
            background-color: rgb(100, 100, 100);
            .menu2 {
                border-radius: 50%;
                background-color: #ddaf2d;
                width: 35px;
                height: 35px;
                position: absolute;
                top: 1%;
                right: 2%;
                text-align: center;
                image {
                    width: 70%;
                    height: 70%;
                    top: 15%;
                }
            }
            .bottom_menu {
                display: flex;
                flex-wrap: wrap;
                justify-content: space-between;
                width: 90%;
                // height: 40%;
                margin: 30rpx auto 0;
                .fot_title {
                    width: 44%;

                    height: 70px;
                    // 渐变灰色
                    background-image: linear-gradient(
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgba(182, 182, 182, 0.8),
                        rgba(182, 182, 182, 0.7),
                        rgba(182, 182, 182, 0.8),
                        rgba(59, 59, 59, 0.5)
                    );
                    border-radius: 10px;
                    position: relative;
                    margin-right: 10rpx;
                    margin-bottom: 30rpx;
                    .title_box {
                        text-align: center;
                        color: #000;
                        font-size: 15px;
                        padding: 8rpx;
                    }
                    .title_status {
                        text-align: center;
                        color: #fff;
                        font-size: 12px;
                        border-radius: 0 0 10px 10px;
                        background-color: #000;
                        height: 23px;
                        line-height: 23px;
                        position: absolute;
                        width: 100%;
                        bottom: 0;
                    }
                    .title_status2 {
                        text-align: center;
                        color: #000;
                        font-size: 12px;
                        border-radius: 0 0 10px 10px;
                        background-color: #ddaf2d;
                        height: 23px;
                        line-height: 23px;
                        position: absolute;
                        width: 100%;
                        bottom: 0;
                    }
                }
            }
            .top_menu {
                display: flex;
                flex-wrap: wrap;
                width: 90%;
                height: 40%;
                margin: 90rpx auto 0;
                // background-color: pink;
                .nav_box {
                    display: flex;
                    width: 50%;
                    height: 100rpx;
                    text-align: center;
                    line-height: 42rpx;
                    color: #ffffff;

                    .nav_box_img {
                        width: 16%;
                        height: 100%;
                    }
                    .nav_box_msg {
                        width: 60%;
                    }
                    .nav_box_msg view:nth-child(1) {
                        font-size: 13px;
                    }
                    .nav_box_msg view:nth-child(2) {
                        font-size: 13px;
                    }
                }
            }
        }
        .menu1 {
            border-radius: 50%;
            background-color: #ddaf2d;
            width: 35px;
            height: 35px;
            position: absolute;
            top: 1%;
            left: 2%;
            text-align: center;
            image {
                width: 70%;
                height: 70%;
                top: 15%;
            }
        }
    }
    .first {
        padding: 52rpx;
        padding-top: 106rpx;
        background-color: pink;
        background-image: linear-gradient(
                rgba(182, 182, 182, 0.5),
                rgba(182, 182, 182, 0.5),
                rgba(59, 59, 59, 0.5),
                rgba(9, 9, 9, 0.5),
                rgba(9, 9, 9, 0.5),
                rgba(9, 9, 9, 0.8),
                rgba(0, 0, 0, 0.9)
            ),
            url(../../static/img/index.png);
        background-size: 100% 100%;
        background-repeat: no-repeat;
        height: 100vh;
        .menu_box {
            width: 60%;
            height: 100vh;
            position: absolute;
            left: 0;
            top: 0;
            z-index: 99;
            background-color: rgb(100, 100, 100);
            .menu2 {
                border-radius: 50%;
                background-color: #ddaf2d;
                width: 35px;
                height: 35px;
                position: absolute;
                top: 1%;
                right: 2%;
                text-align: center;
                image {
                    width: 70%;
                    height: 70%;
                    top: 15%;
                }
            }
            .bottom_menu {
                display: flex;
                flex-wrap: wrap;
                justify-content: space-between;
                width: 90%;
                // height: 40%;
                margin: 30rpx auto 0;
                .fot_title {
                    width: 44%;

                    height: 70px;
                    // 渐变灰色
                    background-image: linear-gradient(
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgb(226, 226, 226),
                        rgba(182, 182, 182, 0.8),
                        rgba(182, 182, 182, 0.7),
                        rgba(182, 182, 182, 0.8),
                        rgba(59, 59, 59, 0.5)
                    );
                    border-radius: 10px;
                    position: relative;
                    margin-right: 10rpx;
                    margin-bottom: 30rpx;
                    .title_box {
                        text-align: center;
                        color: #000;
                        font-size: 15px;
                        padding: 8rpx;
                    }
                    .title_status {
                        text-align: center;
                        color: #fff;
                        font-size: 12px;
                        border-radius: 0 0 10px 10px;
                        background-color: #000;
                        height: 23px;
                        line-height: 23px;
                        position: absolute;
                        width: 100%;
                        bottom: 0;
                    }
                    .title_status2 {
                        text-align: center;
                        color: #000;
                        font-size: 12px;
                        border-radius: 0 0 10px 10px;
                        background-color: #ddaf2d;
                        height: 23px;
                        line-height: 23px;
                        position: absolute;
                        width: 100%;
                        bottom: 0;
                    }
                }
            }
            .top_menu {
                display: flex;
                flex-wrap: wrap;
                width: 90%;
                height: 40%;
                margin: 90rpx auto 0;
                // background-color: pink;
                .nav_box {
                    display: flex;
                    width: 50%;
                    height: 100rpx;
                    text-align: center;
                    line-height: 42rpx;
                    color: #ffffff;

                    .nav_box_img {
                        width: 16%;
                        height: 100%;
                    }
                    .nav_box_msg {
                        width: 60%;
                    }
                    .nav_box_msg view:nth-child(1) {
                        font-size: 13px;
                    }
                    .nav_box_msg view:nth-child(2) {
                        font-size: 13px;
                    }
                }
            }
        }
        .menu1 {
            border-radius: 50%;
            background-color: #ddaf2d;
            width: 35px;
            height: 35px;
            position: absolute;
            top: 1%;
            left: 2%;
            text-align: center;
            image {
                width: 70%;
                height: 70%;
                top: 15%;
            }
        }

        .details_msg {
            width: 80%;
            height: 90%;
            margin: 0 auto;
            position: absolute;
            top: 3%;
            z-index: 99;
            background-color: rgba(9, 9, 9, 0.9);
            padding: 20rpx 30rpx 20rpx 30rpx;
            color: #fff;
            .detalis_colse {
                color: #000;

                float: right;
                border-radius: 50%;
                width: 50rpx;
                height: 50rpx;
                font-weight: bold;
                text-align: center;
                line-height: 50rpx;
                font-size: 27px;
                background-color: #ddaf2d;
            }
            .details_chiness_msg {
                margin-top: 56rpx;
                font-size: 12px;
                margin-bottom: 20rpx;
            }
            .detials_egls_msg {
                font-size: 12px;
            }
            .close2 {
                width: 100rpx;
                padding: 10rpx;
                font-size: 12px;
                background-color: #ddaf2d;
                color: #000;
                text-align: center;
                border-radius: 100rpx;
                margin-top: 10rpx;
                margin: 0 auto;
                position: absolute;
                bottom: 5%;
                left: 50%;
                transform: translateX(-50%);
            }
        }
        .movie_msg {
            padding: 20rpx;
            .chiness_msg {
                font-size: 12px;
                color: #ffffff;
                margin-bottom: 15rpx;
            }
            .egls_msg {
                font-size: 13px;
                color: #ffffff;
            }
            .more_msg {
                text-align: right;
                color: #ddaf2d;
            }
        }
        .movie_title {
            font-size: 30rpx;
            color: #ddaf2d;
            font-weight: bold;
            font-size: 18px;
            margin: 20rpx 0;
        }
        .movie_title2 {
            font-size: 30rpx;
            color: #ddaf2d;
            font-weight: bold;
            font-size: 12px;
            margin: 20rpx 0;
        }
        .movie_address {
            color: #ffffff;
            font-size: 13px;
            margin-top: 5rpx;
        }
        .footer_box {
            margin-top: 70rpx;
            width: 100%;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            .fot_title {
                width: 20%;
                height: 70px;
                // 渐变灰色
                background-image: linear-gradient(
                    rgb(226, 226, 226),
                    rgb(226, 226, 226),
                    rgb(226, 226, 226),
                    rgb(226, 226, 226),
                    rgb(226, 226, 226),
                    rgb(226, 226, 226),
                    rgb(226, 226, 226),
                    rgba(182, 182, 182, 0.8),
                    rgba(182, 182, 182, 0.7),
                    rgba(182, 182, 182, 0.8),
                    rgba(59, 59, 59, 0.5)
                );
                border-radius: 10px;
                position: relative;
                margin-right: 10rpx;
                margin-bottom: 30rpx;
                .title_box {
                    text-align: center;
                    color: #000;
                    font-size: 15px;
                    padding: 8rpx;
                }
                .title_status {
                    text-align: center;
                    color: #fff;
                    font-size: 12px;
                    border-radius: 0 0 10px 10px;
                    background-color: #000;
                    height: 23px;
                    line-height: 23px;
                    position: absolute;
                    width: 100%;
                    bottom: 0;
                }
                .title_status2 {
                    text-align: center;
                    color: #000;
                    font-size: 12px;
                    border-radius: 0 0 10px 10px;
                    background-color: #ddaf2d;
                    height: 23px;
                    line-height: 23px;
                    position: absolute;
                    width: 100%;
                    bottom: 0;
                }
            }
        }

        .icon_swiper {
            width: 100%;
            height: 90rpx;
            // display: flex;
            padding: 10rpx 0 10rpx 0;
            background-color: rgb(99, 99, 99);
            white-space: nowrap;
            overflow: hidden;
            position: relative;

            .left_icon {
                width: 5%;
                height: 50%;
                line-height: 90rpx;
                color: rgb(141, 141, 141);
                line-height: 100rpx;
                font-size: 16px;
                position: absolute;
                left: 0;
                top: 50%;
                transform: translateY(-50%);
                image {
                    width: 100%;
                    height: 30%;
                }
                // /deep/uni-image > img {
                //     -webkit-touch-callout: none;
                //     -webkit-user-select: none;
                //     -moz-user-select: none;
                //     /* display: block; */
                //     /* position: absolute; */
                //     /* top: 0; */
                //     /* left: 0; */
                //     opacity: 1;
                // }
            }
            .right_icon {
                width: 5%;
                height: 50%;
                line-height: 90rpx;
                color: rgb(141, 141, 141);
                line-height: 100rpx;
                font-size: 16px;
                position: absolute;
                right: 0;
                top: 50%;
                transform: translateY(-50%);
                image {
                    width: 100%;
                    height: 30%;
                }
                // /deep/uni-image > img {
                //     -webkit-touch-callout: none;
                //     -webkit-user-select: none;
                //     -moz-user-select: none;
                //     /* display: block; */
                //     /* position: absolute; */
                //     /* top: 0; */
                //     /* left: 0; */
                //     opacity: 1;
                // }
            }
            .icon_new {
                width: 87%;
                margin: 0 auto;
                // display: flex;
                // justify-content: space-around;
                // flex-wrap: wrap;
                overflow: hidden;
                scroll-behavior: smooth;
                .icons_box1 {
                    width: 16%;
                    height: 90rpx;
                    margin: 0 10rpx 0 10rpx;
                    display: inline-block;
                }
                .icons_box {
                    width: 17%;
                    height: 100%;
                    image {
                        width: 100%;
                        height: 100%;
                    }
                    /deep/uni-image > img {
                        -webkit-touch-callout: none;
                        -webkit-user-select: none;
                        -moz-user-select: none;
                        /* display: block; */
                        /* position: absolute; */
                        /* top: 0; */
                        /* left: 0; */
                        opacity: 1;
                    }
                }
            }

            // .swiper-slide {
            //     text-align: center;
            //     font-size: 18px;
            //     background: #fff;
            //     display: -webkit-box;
            //     display: -ms-flexbox;
            //     display: -webkit-flex;
            //     display: flex;
            //     -webkit-box-pack: center;
            //     -ms-flex-pack: center;
            //     -webkit-justify-content: center;
            //     justify-content: center;
            //     -webkit-box-align: center;
            //     -ms-flex-align: center;
            //     -webkit-align-items: center;
            //     align-items: center;
            // }
        }
        .box_swiper {
            width: 100%;
            height: 60px;
            // margin: 0 auto;
            image {
                width: 40%;
                height: 100%;
            }
        }
        .top_hot_box {
            display: flex;
            height: 70rpx;
            justify-content: flex-end;
            align-items: center;
            padding: 30rpx 0 30rpx 0;
            margin-top: 20rpx;
            .hot_heart {
                width: 27%;
                height: 100%;
                display: flex;
                align-items: center;
                justify-content: space-between;
                .hot_num {
                    width: 50%;
                    color: #ffffff;
                }
                .heart_img {
                    width: 40%;
                    height: 100%;
                    image {
                        width: 100%;
                        height: 100%;
                    }
                }
            }
        }
    }
    .page {
        width: 100%;
        height: 100vh;
    }

    .uni-padding-wrap {
        width: 100%;
        height: 100%;
        padding: 0;
    }

    .swiper1 {
        width: 100%;
        height: 100vh;
    }

    .xiala_img {
        height: 56upx;
        width: 56upx;
        position: absolute;
        bottom: 10upx;
        left: 338upx;
    }

    .noMorePages {
        width: 100%;
        text-align: center;
        height: 56upx;
        line-height: 56upx;
        position: absolute;
        bottom: 10upx;
        color: #333;
    }
</style>
