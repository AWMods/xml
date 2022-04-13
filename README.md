<?xml version="1.0" encoding="utf-8" ?>
<FrameLayout xmlns:android="http://schemas.android.com/apk/res/android" android:layout_width="fill_parent" android:layout_height="fill_parent">
	<com.whatsapp.components.MainChildCoordinatorLayout xmlns:android="http://schemas.android.com/apk/res/android" xmlns:app="http://schemas.android.com/apk/res-auto" android:layout_width="fill_parent" android:layout_height="fill_parent" app:mcclChildId="@id/bottom_sheet">
		<FrameLayout android:id="@id/content_sheet" android:layout_width="fill_parent" android:layout_height="fill_parent">
			<FrameLayout android:id="@id/content" android:layout_width="fill_parent" android:layout_height="fill_parent" />
			<com.whatsapp.WaTextView android:textSize="22.0sp" android:textColor="@color/white" android:gravity="center" android:id="@id/error" android:padding="16.0dip" android:visibility="gone" android:layout_width="fill_parent" android:layout_height="fill_parent" />
			<View android:id="@id/click_handler" android:layout_width="fill_parent" android:layout_height="fill_parent" />
			<LinearLayout android:layout_gravity="bottom" android:orientation="vertical" android:id="@id/caption_container" android:layout_width="fill_parent" android:layout_height="wrap_content">
				<FrameLayout android:layout_gravity="bottom" android:orientation="vertical" android:layout_width="fill_parent" android:layout_height="wrap_content">
					<LinearLayout android:layout_gravity="bottom" android:orientation="vertical" android:layout_width="fill_parent" android:layout_height="wrap_content">
						<com.whatsapp.ui.media.MediaCaptionTextView android:textSize="18.0sp" android:textColor="@color/white" android:layout_gravity="bottom" android:id="@id/caption" android:paddingLeft="16.0dip" android:paddingTop="10.0dip" android:paddingRight="16.0dip" android:paddingBottom="20.0dip" android:visibility="gone" android:layout_width="fill_parent" android:layout_height="wrap_content" android:shadowColor="@color/black" android:shadowDx="1.0" android:shadowDy="1.0" android:shadowRadius="2.5" android:lineSpacingMultiplier="1.12" app:rmtvLines="3" app:rmtvLinkBold="true" app:rmtvLinkColor="@color/white" app:rmtvText="@string/read_more" />
						<View android:id="@id/caption_padding" android:background="@color/white" android:layout_width="fill_parent" android:layout_height="1.0dip" android:layout_marginLeft="15.0dip" android:layout_marginTop="0.0dip" android:layout_marginRight="15.0dip" android:layout_marginBottom="90.0dip" android:alpha="0.7" />
					</LinearLayout>
					<RelativeLayout android:layout_gravity="bottom" android:paddingBottom="10.0dip" android:layout_width="fill_parent" android:layout_height="40.0dip">
						<ImageView android:id="@id/div" android:layout_width="40.0dip" android:layout_height="40.0dip" android:src="@drawable/message_got_receipt_from_target_onmedia" android:layout_alignParentLeft="true" android:layout_alignParentStart="true" />
						<ImageView android:layout_gravity="end" android:id="@id/div2" android:layout_width="40.0dip" android:layout_height="40.0dip" android:src="@drawable/ic_downloadstatus" android:layout_alignParentRight="true" android:layout_alignParentEnd="true" />
					</RelativeLayout>
				</FrameLayout>
			</LinearLayout>
			<FrameLayout android:layout_gravity="center" android:id="@id/control_frame" android:background="@drawable/download_background" android:visibility="gone" android:layout_width="wrap_content" android:layout_height="wrap_content">
				<com.whatsapp.CircularProgressBar android:layout_gravity="center" android:id="@id/progress_bar" android:visibility="gone" android:layout_width="64.0dip" android:layout_height="64.0dip" android:indeterminateOnly="false" app:cpbBackground="@color/transparent" app:cpbColor="@color/white_alpha_60" app:cpbFill="@color/transparent" app:cpbOutlineColor="@color/black_alpha_10" app:cpbOutlineWidth="1.0dip" app:cpbStrokeWidthFactor="5.0" />
				<com.whatsapp.WaImageView android:layout_gravity="center" android:id="@id/cancel_btn" android:visibility="gone" android:layout_width="wrap_content" android:layout_height="wrap_content" android:src="@drawable/btn_cancel" />
				<com.whatsapp.WaButton android:id="@id/control_btn" android:text="@string/button_download" style="@style/ConversationRowControlButton.Left" />
			</FrameLayout>
			<View android:id="@id/status_details_background" android:background="@color/black_alpha_40" android:visibility="gone" android:layout_width="fill_parent" android:layout_height="fill_parent" />
		</FrameLayout>
		<LinearLayout android:orientation="vertical" android:id="@id/bottom_sheet" android:paddingTop="96.0dip" android:paddingBottom="144.0dip" android:layout_width="fill_parent" android:layout_height="wrap_content" app:behavior_peekHeight="@dimen/status_footer_peek_height" app:layout_behavior="com.google.android.material.bottomsheet.BottomSheetBehavior">
			<FrameLayout android:layout_gravity="center_horizontal" android:id="@id/info" android:background="@drawable/ic_center_shadow" android:layout_width="wrap_content" android:layout_height="76.0dip">
				<com.whatsapp.WaTextView android:textSize="13.0sp" android:textColor="@color/white" android:layout_gravity="bottom|center" android:id="@id/info_btn" android:paddingTop="0.0dip" android:paddingBottom="10.0dip" android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_marginBottom="30.0dip" android:minHeight="0.0dip" android:text="@string/info" android:shadowColor="@color/black_alpha_45" android:shadowDx="0.0" android:shadowDy="0.0" android:shadowRadius="3.0" android:drawableTop="@drawable/ic_ptt_lock_arrow" android:textAllCaps="true" android:drawableTint="@android:color/white" style="@style/ActionBarButtonStyle" />
				<androidx.recyclerview.widget.RecyclerView android:scrollbars="none" android:layout_width="fill_parent" android:layout_height="wrap_content" />
			</FrameLayout>
			<FrameLayout android:id="@id/extra_padding" android:layout_width="fill_parent" android:layout_height="wrap_content" />
		</LinearLayout>
	</com.whatsapp.components.MainChildCoordinatorLayout>
</FrameLayout>
