# How to center align the Expander header text in Xamarin.Forms (SfExpander)?

You can center align the text of the Expander [Header](https://help.syncfusion.com/cr/cref_files/xamarin/Syncfusion.Expander.XForms~Syncfusion.XForms.Expander.SfExpander~Header.html?) in Xamarin.Forms [SfExpander](https://help.syncfusion.com/xamarin/expander/getting-started?) by using the [HorizontalTextAlignment](https://docs.microsoft.com/en-us/dotnet/api/xamarin.forms.label.horizontaltextalignment?view=xamarin-forms) and [VerticalTextAlignment](https://docs.microsoft.com/en-us/dotnet/api/xamarin.forms.label.verticaltextalignment?view=xamarin-forms) properties.

You can refer the following article.

https://www.syncfusion.com/kb/11360/how-to-center-align-the-expander-header-text-in-xamarin-forms-sfexpander 


**XAML**

Set **HorizontalTextAlignment** and **VerticalTextAlignment** of the header label to **Center**.

``` xml
<ContentPage xmlns="http://xamarin.com/schemas/2014/forms"
             xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
             xmlns:syncfusion="clr-namespace:Syncfusion.XForms.Expander;assembly=Syncfusion.Expander.XForms"
             x:Class="ExpanderXamarin.MainPage">
    <ContentPage.Content>
        <ScrollView BackgroundColor="#EDF2F5">
            <StackLayout>
                <syncfusion:SfExpander>
                    <syncfusion:SfExpander.Header>
                        <Grid HeightRequest="50">
                            <Label Text="Veg Pizza" TextColor="#495F6E" VerticalTextAlignment="Center" HorizontalTextAlignment="Center"/>
                        </Grid>
                    </syncfusion:SfExpander.Header>
                    <syncfusion:SfExpander.Content>
                        <Grid Padding="10,10,10,10" BackgroundColor="#FFFFFF">
                            <Label BackgroundColor="#FFFFFF" HeightRequest="50" Text="Veg pizza is prepared with the items that meet vegetarian standards by not including any meat or animal tissue products." TextColor="#303030" VerticalTextAlignment="Center"/>
                        </Grid>
                    </syncfusion:SfExpander.Content>
                </syncfusion:SfExpander>

                <syncfusion:SfExpander>
                    <syncfusion:SfExpander.Header>
                        <Grid HeightRequest="50">
                            <Label Text="Non-veg Pizza" TextColor="#495F6E" VerticalTextAlignment="Center" HorizontalTextAlignment="Center"/>
                        </Grid>
                    </syncfusion:SfExpander.Header>
                    <syncfusion:SfExpander.Content>
                        <Grid Padding="10,10,10,10" BackgroundColor="#FFFFFF">
                            <Label Text="Non-veg pizza is prepared by including the meat and animal tissue products." HeightRequest="50" TextColor="#303030" VerticalTextAlignment="Center"/>
                        </Grid>
                    </syncfusion:SfExpander.Content>
                </syncfusion:SfExpander>
            </StackLayout>
        </ScrollView>
    </ContentPage.Content>
</ContentPage>
```
**Output**

![HeaderCenterAlign](https://github.com/SyncfusionExamples/expander-header-center-align-xamarin/blob/master/ScreenShots/HeaderCenterAlign.jpg)
