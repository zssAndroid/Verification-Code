# VerificationCodeInput
[![](https://jitpack.io/v/liuguangli/VerificationCodeInput.svg)](https://jitpack.io/#liuguangli/VerificationCodeInput)

简洁验证码输入框，能自定义输入框个数和样式。

![](https://github.com/liuguangli/VerificationCodeInput/blob/master/verification1.gif)

# How to use
    <com.dalimao.corelibrary.VerificationCodeInput
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            ver:box="4"
            ver:child_h_padding="5dp"
            android:layout_centerInParent="true"
            android:id="@+id/verificationCodeInput"
            android:layout_marginBottom="16dp"
            />

监听输入完成：

    VerificationCodeInput input = (VerificationCodeInput) findViewById(R.id.verificationCodeInput);
    input.setOnCompleteListener(new VerificationCodeInput.Listener() {
          @Override
          public void onComplete(String content) {
             Log.d(TAG, "完成输入：" + content);
          }
    });

你还可以为输入框定义自己的样式，指定属性 box_bg_normal 和 box_bg_focus：

    <com.dalimao.corelibrary.VerificationCodeInput
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            ver:box="4"
            ver:box_bg_normal="@drawable/verification_edit_bg_normal"
            ver:box_bg_focus="@drawable/verification_edit_bg_focus"
            ver:child_h_padding="5dp"
            android:layout_centerInParent="true"
            android:layout_marginBottom="16dp"
            />

自定义个数，指定属性  box：

    <com.dalimao.corelibrary.VerificationCodeInput
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            ver:box="5"
            ver:box_bg_normal="@drawable/verification_edit_bg_normal"
            ver:box_bg_focus="@drawable/verification_edit_bg_focus"
            ver:child_h_padding="5dp"
            android:layout_centerInParent="true"
            android:layout_marginBottom="16dp"
            />

自定义输入类型：指定属性 inputType：

     <com.dalimao.corelibrary.VerificationCodeInput
         android:layout_width="wrap_content"
         android:layout_height="wrap_content"
         ver:box="5"
         ver:box_bg_normal="@drawable/verification_edit_bg_normal"
         ver:box_bg_focus="@drawable/verification_edit_bg_focus"
         ver:child_h_padding="5dp"
         ver:inputType="password"
         android:layout_centerInParent="true"
         android:layout_marginBottom="16dp"
         />

![](https://github.com/liuguangli/VerificationCodeInput/blob/master/verification.gif).
