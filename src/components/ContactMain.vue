<template>
    <!-- メイン -->
    <main>
        <div class="container">
        <h2>Contact</h2>
        <p>カフェ Mr. M COFFEE（ミスターエムコーヒー）へのお問合せ、こちらのフォームをご利用ください。</p>
        </div>
        <!-- お問合せフォーム -->
        <div class="py-3">
            <div class="container">
                <h3 class="mb-3">お問合せフォーム</h3>
                    <!-- フォーム -->
                    <form action="" method="POST">
                    <!-- お名前 -->
                    <div class="form-group row">
                        <label htmlFor="your_name" class="col-md-3 col-form-label">
                            お名前 <span class="badge badge-warning">必須</span>
                        </label>
                        <div class="col-md-9">
                            <!-- 該当する入力値(POSTパラメータ)が空じゃない場合のみ、入力値をvalue属性にセット -->
                            <input type="text" name="your_name" id="your_name" class="form-control" required defaultValue="" />
                        </div>
                    </div>
                    <!-- メールアドレス -->
                    <div class="form-group row">
                        <label htmlFor="email" class="col-md-3 col-form-label">
                            メールアドレス <span class="badge badge-warning">必須</span>
                        </label>
                        <div class="col-md-9">
                            <!-- 該当する入力値(POSTパラメータ)が空じゃない場合のみ、入力値をvalue属性にセット -->
                            <input type="email" id="email" class="form-control" required name="email" defaultValue="" />
                        </div>
                    </div>
                    <!-- きっかけ -->
                    <fieldset class="form-group">
                        <div class="row">
                            <label htmlFor="radio" class="col-md-3 col-form-label">
                                Mr. M COFFEEを知ったきっかけ
                            </label>
                            <div class="col-md-9">
                                <div class="form-check form-check-inline">
                                    <!-- 該当する入力値(POSTパラメータ)が空じゃない場合のみ、入力値をvalue属性にセット -->
                                    <input type="radio" name="questionnaire" id="radio radio1" class="form-check-input" defaultValue="answer1" />
                                    <label htmlFor="radio1" class="form-check-label">口コミ</label>
                                </div>
                                <div class="form-check form-check-inline">
                                    <!-- 該当する入力値(POSTパラメータ)が空じゃない場合のみ、入力値をvalue属性にセット -->
                                    <input type="radio" name="questionnaire" id="radio radio2" class="form-check-input" defaultValue="answer2" />
                                    <label htmlFor="radio2" class="form-check-label">検索エンジン</label>
                                </div>
                                <div class="form-check form-check-inline">
                                    <!-- 該当する入力値(POSTパラメータ)が空じゃない場合のみ、入力値をvalue属性にセット -->
                                    <input type="radio" name="questionnaire" id="radio radio3" class="form-check-input" defaultValue="answer3" />
                                    <label htmlFor="radio3" class="form-check-label">広告</label>
                                </div>
                            </div>
                        </div>
                    </fieldset>
                    <!-- 種類 -->
                    <div class="form-group row">
                        <label htmlFor="category" class="col-md-3 col-form-label">
                            お問い合わせ種類 <span class="badge badge-warning">必須</span>
                        </label>
                        <div class="col-md-9">
                            <select name="category" id="category" class="form-control">
                                <option value="">選択してください</option>
                                <!-- 該当する入力値(POSTパラメータ)が空じゃない場合のみ、入力値をvalue属性にセット -->
                                <option value="1">ご予約について</option>
                                <!-- 該当する入力値(POSTパラメータ)が空じゃない場合のみ、入力値をvalue属性にセット -->
                                <option value="2">委託販売について</option>
                                <!-- 該当する入力値(POSTパラメータ)が空じゃない場合のみ、入力値をvalue属性にセット -->
                                <option value="3">その他のお問い合わせ</option>
                            </select>
                        </div>
                    </div>
                    <!-- 内容 -->
                    <div class="form-group row">
                        <label htmlFor="contact" class="col-md-3 col-form-label">
                            お問い合わせ内容 <span class="badge badge-warning">必須</span>
                        </label>
                        <div class="col-md-9">
                            <textarea name="contact" id="contact" rows="8" class="form-control" defaultValue="" />
                        </div>
                    </div>
                    <!-- 確認ボタン -->
                    <div class="form-group row justify-content-end">
                        <div class="col-md-9">
                            <input type="submit" name="btn_confilm" class="btn btn-primary" defaultValue="確認する" />
                        </div>
                    </div>
                </form>
                <!-- /フォーム -->
            </div>
        </div>
        <!-- /お問合せフォーム -->
    </main>
    <!-- /メイン -->
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class ContactMain extends Vue {}
</script>