<template>
    <view class="page">
        <view class="uni-padding-wrap">
            <view class="page-section swiper1">
                <view class="page-section-spacing">
                    <!-- page1 -->
                    <swiper class="swiper1" vertical="true">
                        <swiper-item v-for="item in 4" :key="item">
                            <view class="swiper-item">
                                <view class="first">
                                    <view class="box_swiper">
                                        <u-swiper
                                            :circular="true"
                                            height="267rpx"
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
                                            <image
                                                v-for="(item, index) in iconArr"
                                                :key="index"
                                                class="icons_box1"
                                                :src="item.imgUrl"></image>
                                            <!-- <image class="icons_box1" src="../../static/img/1.png"></image>
                                            <image class="icons_box1" src="../../static/img/2.png"></image>
                                            <image class="icons_box1" src="../../static/img/3.png"></image>
                                            <image class="icons_box1" src="../../static/img/4.png"></image>
                                            <image class="icons_box1" src="../../static/img/5.png"></image>
                                            <image class="icons_box1" src="../../static/img/5.png"></image>
                                            <image class="icons_box1" src="../../static/img/5.png"></image> -->
                                        </view>
                                    </view>
                                    <view class="movie_title" @click="goDetails">?????????????????????</view>
                                    <view class="movie_title2"
                                        >PINGYAO CROUCHING TIGER HIDDEN DRAGON INTERNATIONAL FILM FESTIVAL</view
                                    >
                                    <view class="movie_year_num">
                                        <view>??????</view>
                                        <view>??????</view>
                                    </view>
                                    <view class="movie_startTime">???????????????2022???10???8???</view>
                                    <view class="movie_endTime">???????????????2022???10???16???</view>
                                    <view class="movie_address">????????????????????? ?????? ??????</view>
                                    <view class="footer_box">
                                        <view class="fot_title">
                                            <view class="title_box">?????? <br />??????</view>
                                            <view class="title_status">?????????</view>
                                        </view>
                                        <view class="fot_title">
                                            <view class="title_box">?????? <br />??????</view>
                                            <view class="title_status2">?????????</view>
                                        </view>
                                        <view class="fot_title">
                                            <view class="title_box">?????? <br />??????</view>
                                            <view class="title_status">?????????</view>
                                        </view>
                                        <view class="fot_title">
                                            <view class="title_box">?????? <br />??????</view>
                                            <view class="title_status">?????????</view>
                                        </view>
                                        <view class="fot_title">
                                            <view class="title_box">?????? <br />??????</view>
                                            <view class="title_status">?????????</view>
                                        </view>
                                        <view class="fot_title">
                                            <view class="title_box">?????? <br />??????</view>
                                            <view class="title_status2">?????????</view>
                                        </view>
                                        <view class="fot_title">
                                            <view class="title_box">?????? <br />??????</view>
                                            <view class="title_status">?????????</view>
                                        </view>
                                        <view class="fot_title">
                                            <view class="title_box">?????? <br />??????</view>
                                            <view class="title_status">?????????</view>
                                        </view>
                                    </view>
                                </view>
                            </view>
                        </swiper-item>
                        <!-- <swiper-item>
                            <view class="swiper-item"> ????????? </view>
                        </swiper-item>
                        <swiper-item>
                            <view class="swiper-item"> ???????????? </view>
                            <view class="noMorePages"> ??????????????????????????? </view>
                        </swiper-item> -->
                    </swiper>
                </view>
            </view>
        </view>
    </view>
</template>

<script>
    // import Swiper from '@/node_modules/swiper/swiper-bundle'; // ??????swiper
    // import '@/node_modules/swiper/swiper-bundle.min.css';

    export default {
        name: '',
        // ????????????
        data() {
            return {
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

                swiper: [
                    {
                        url: '../../static/img/banner.jpg',
                        title: '??????1',
                    },
                    {
                        url: '../../static/img/banner2.jpg',
                        title: '??????2',
                    },
                    {
                        url: '../../static/img/banner3.jpg',
                        title: '??????3',
                    },
                ],
            };
        },
        /*
      ????????????????????????
    */
        onLoad() {},
        /*
      ??????????????????????????????
    */
        onShow() {
            // var mySwiper = new Swiper('.swiper', {
            //     direction: 'horizontal', // ??????????????????
            //     // loop: true, // ??????????????????
            //     slidesPerView: 3,
            //     // ?????????????????????
            //     // pagination: {
            //     //     el: '.swiper-pagination',
            //     // },
            //     // ??????????????????????????????
            //     navigation: {
            //         nextEl: '.swiper-button-next',
            //         prevEl: '.swiper-button-prev',
            //     },
            //     // ?????????????????????
            //     // scrollbar: {
            //     //     el: '.swiper-scrollbar',
            //     // },
            // });
        },
        /*
      ??????????????????
    */
        mounted() {
            if (document != undefined) {
                document.getElementsByClassName('uni-placeholder')[0].style.display = 'none';
                document.getElementsByClassName('uni-page-head')[0].style.display = 'none';
            }
        },
        methods: {
            goDetails() {
                uni.navigateTo({
                    url: '/pages/tabBarA/tabBarA',
                });
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
                // ???????????? ??? ????????????
                if (LOR) {
                    // ??????1???????????????????????????????????????????????????????????????????????????
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
                // ?????? items ????????????????????????
                let first = this.iconArr[0];
                // ????????????????????????????????????
                this.iconArr.splice(0, 1);
                // ??????????????????????????????????????????
                this.iconArr.push(first);
                // ????????????
                // this.$refs.tagsP.scrollLeft = this.scrollNum;
                let distance = this.$refs.tagsP.scrollLeft;

                let scrollNum = distance + 200;
                let step = (distance - scrollNum) / 50;
                if (step < 0) step = -step;
                this.moveSlow(distance, scrollNum, step, true);
            },
            toLeft() {
                // ?????? items ???????????????????????????
                let last = this.iconArr[this.iconArr.length - 1];
                // ???????????????????????????????????????
                this.iconArr.splice(this.iconArr.length - 1, 1);
                // ?????????????????????????????????????????????
                this.iconArr.unshift(last);
                // ?????????
                // let distance = this.$refs.tagsP.scrollLeft;
                // let scrollNum = distance - 200;
                // if (scrollNum < 0) {
                //     scrollNum = 0;
                // }
                // let step = (distance - scrollNum) / 50;
                // if (step < 0) step = -step;
                // this.moveSlow(distance, scrollNum, step, false);
            },
            // toLeft() {
            //
            //     // ???????????????????????????icons_box1??????????????????????????????????????????
            //     var icons_box = document.getElementsByClassName('icons_box');
            //     for (var i = 0; i < icons_box.length; i++) {
            //         icons_box[i].style.transform = 'translateX(' + 50 * (i + 1) + 'px)';
            //     }
            // },
            // toRight() {
            //

            //     // ???????????????????????????icons_box??????????????????????????????????????????
            //     var icons_box = document.getElementsByClassName('icons_box');
            //     for (var i = 0; i < icons_box.length; i++) {
            //         icons_box[i].style.transform = 'translateX(' + 50 * (i - 1) + 'px)';
            //     }
            // },
            change(e) {},
            click(e) {
                // ??????????????????
                // uni.previewImage({
                //     current: e.url, // ?????????????????????http??????
                //     urls: [e.url], // ?????????????????????http????????????
                // });
            },
        },
        /*
      ??????????????????????????????
    */
        onReady() {},
        /*
      ????????????????????????
    */
        onHide() {},
        /*
      ??????????????????
    */
        onUnload() {},
        /*
      ????????????????????????
    */
        onResize() {},
        /*
      ????????????????????????
    */
        onPullDownRefresh() {},
        /*
      ??????????????????????????????
    */
        onReachBottom() {},
        /*
      ?????? tab ?????????
    */
        onTabItemTap() {},
        /*
      ???????????????????????????
    */
        onShareAppMessage() {},
        /*
      ??????????????????
    */
        onPageScroll() {},
        /*
      ????????????
    */
        components: {},
        /*
      ?????????
    */
        watch: {},
        /*
      ????????????
    */
        computed: {},
    };
</script>

<style lang="scss" scoped>
    .first {
        padding: 40rpx;
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
        display: flex;
        flex-direction: column;
        justify-content: center;
        .footer_box {
            margin-top: 70rpx;
            width: 100%;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            .fot_title {
                width: 20%;
                height: 70px;
                // ????????????
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
        .movie_title {
            font-size: 30rpx;
            color: #ddaf2d;
            font-weight: bold;
            font-size: 18px;
            margin: 20rpx 0;
            letter-spacing: 3px;
        }
        .movie_title2 {
            font-size: 30rpx;
            color: #ddaf2d;
            // font-weight: bold;
            font-size: 12px;
            // margin: 20rpx 0;
        }
        .movie_year_num {
            display: flex;
            align-items: center;
        }
        .movie_year_num view:nth-child(1) {
            background-color: #ddaf2d;
            color: #000;
            width: 100rpx;
            text-align: center;
            padding: 5rpx;
            font-size: 13px;
        }
        .movie_year_num view:nth-child(2) {
            background-color: #ddaf2d;
            color: #000;
            width: 100rpx;
            text-align: center;
            padding: 5rpx;
            margin-left: 10rpx;
            font-size: 13px;
        }
        .movie_startTime {
            color: #ffffff;
            font-size: 13px;
            margin-top: 5rpx;
        }
        .movie_endTime {
            color: #ffffff;
            font-size: 13px;
            margin-top: 5rpx;
        }
        .movie_address {
            color: #ffffff;
            font-size: 13px;
            margin-top: 5rpx;
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
            height: 267rpx;
            // margin: 0 auto;
        }
        .top_hot_box {
            display: flex;
            height: 70rpx;
            justify-content: flex-end;
            align-items: center;
            padding: 30rpx 0 30rpx 0;
            margin-top: 20rpx;
            .hot_heart {
                width: 24%;
                height: 100%;
                display: flex;
                align-items: center;
                justify-content: space-between;
                .hot_num {
                    width: 45%;
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
