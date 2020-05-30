# commondiloag
builder构建弹窗


```
        final CommonDialog dialog = new CommonDialog.Builder(this)
                .setContentView(R.layout.test_dialog_common)
                .setText(R.id.dialog_des, "我是dialog")
                .setText(R.id.cancel, "取消")
                .setText(R.id.confirm, "确定")
                .setCancelable(true)
                .show();
        dialog.setOnClickListener(R.id.confirm, new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Toast.makeText(getApplicationContext(),"确定",Toast.LENGTH_SHORT).show();
                dialog.dismiss();
            }
        });
        dialog.setOnClickListener(R.id.cancel, new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Toast.makeText(getApplicationContext(),"取消",Toast.LENGTH_SHORT).show();
                dialog.dismiss();
            }
        });
```
